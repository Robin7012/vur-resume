<template>
  <div class="page">
    <header>
      <Topbar/>
    </header>
    <main>
      <ResumeEditor/>
      <ResumePreview/>
    </main>
  
  </div>
</template>

<script>
import 'normalize.css/normalize.css'
import './assets/reset.css'
import Topbar from './components/Tobar'
import ResumeEditor from './components/ResumeEditor'
import ResumePreview from './components/ResumePreview'


export default {
  name: 'app',
  data() {
    return {
      text: '你好'
    }
  },
  components: {
    Topbar, ResumeEditor, ResumePreview
  }
}
</script>

<style>
.page {
  height: 100vh;
  display: flex;
  flex-direction: column;
  background: #EAEBEC;
}

.page>main {
  min-width: 1024px;
  max-width: 1440px;
  margin: 0;
  flex-grow: 1;
  display: flex;
  justify-content: space-around;
  margin-top: 16px;
  margin-bottom: 16px;
  width: 100%;
  justify-content: space-between;
  padding: 0 16px;
  align-self: center;
}

#resumeEditor {
  width: 35%;
  background: #444;
}

#resumePreview {
  width: 61.66667%;
  background: #777;
}
</style>
