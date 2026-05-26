<template>
  <div id="app">
    <ejs-documenteditorcontainer
      height="590px"
      :serviceUrl="serviceUrl"
      :enableToolbar="true">
    </ejs-documenteditorcontainer>
  </div>
</template>

<script>
import { DocumentEditorContainerComponent, Toolbar } from '@syncfusion/ej2-vue-documenteditor';

export default {
  name: "App",

  components: {
    "ejs-documenteditorcontainer": DocumentEditorContainerComponent
  },

  data() {
    // Use the following service URL only for demo purposes
    return {
      serviceUrl: 'https://document.syncfusion.com/web-services/docx-editor/api/documenteditor/'
    };
  },

  provide: {
    // Inject required modules.
    DocumentEditorContainer: [Toolbar]
  }
};
</script>

<style>
@import '../node_modules/@syncfusion/ej2-base/styles/material.css';
@import '../node_modules/@syncfusion/ej2-buttons/styles/material.css';
@import '../node_modules/@syncfusion/ej2-inputs/styles/material.css';
@import '../node_modules/@syncfusion/ej2-popups/styles/material.css';
@import '../node_modules/@syncfusion/ej2-lists/styles/material.css';
@import '../node_modules/@syncfusion/ej2-navigations/styles/material.css';
@import '../node_modules/@syncfusion/ej2-splitbuttons/styles/material.css';
@import '../node_modules/@syncfusion/ej2-dropdowns/styles/material.css';
@import '../node_modules/@syncfusion/ej2-vue-documenteditor/styles/material.css';
</style>
