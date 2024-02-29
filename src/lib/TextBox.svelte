<script>
  import EditorJS from "@editorjs/editorjs";
  //@ts-ignore
  import RawTool from "@editorjs/raw";
  //@ts-ignore
  import Header from "@editorjs/header";

  export const textBox = new EditorJS({
    holder: "text",
    tools: {
      header: {
        class: Header,
        config: {
          placeholder: "Enter a header",
          levels: [2, 3, 4],
          defaultLevel: 3,
        },
      },
      raw: RawTool,
    },
  });
</script>

<div class="container">
  <h1>Box</h1>
  <div class="text" id="text"></div>
</div>

<style>
  .container {
    width: 500px;
    text-align: center;
    background-color: gray;
  }

  .text {
    color: #fff;
  }
</style>
