<script>
    export let data = {};
</script>



<style>
body {
  background-color: #ecf0f1 ;
}
blockquote {
  color: #2c3e50;
  font-size: 36px;
  line-height: 150%;
  position: relative;
  font-family: Georgia, serif;
  width: 70%;
  margin: 10% auto;
}
  blockquote::before {
    content: '\201C';
    position: absolute;
    top: -10px;
    left: 0;
    font-family: Arial, sans-serif;
    font-size: 82px;
    font-style: normal;
  }
  blockquote::after {
    content: '\201D';
    position: absolute;
    bottom: -60px;
    right: 0;
    font-family: Arial, sans-serif;
    font-size: 82px;
    font-style: normal;
  }

</style>

<blockquote>
    {data.content}
</blockquote>
