HELLO WORLD

---

# DeEvilizer

Android google で pdf を見るときの邪気を払う。

<input type="url" id="app001-input">
<input type="button" value="DeEvilize" id="app001-button" onclick="callApp001()">
<div id="app001-output" > *** </div>

<script>
const callApp001 = () => {
  console.log("Run callApp001");
  const url = document.getElementById("app001-input").value;
  const searchParams = new URL(url).searchParams;
  const responseText = searchParams.get("url");
  const response = document.getElementById("app001-output");
  response.textContent = responseText;
}
</script>
