HELLO WORLD

---

<input type="url" id="app001" oninput="callApp001"/>
<div id="app001-response" > *** </div>

<script>
const callApp001 = (text) => {
  const url = text;
  const searchParams = new URL(url).searchParams;
  const responseText = searchParams.get("url");
  const response = document.getElementById("app001-response");
  response.text = responseText
}
</script>
