### Hi there 👋<a href="https://github.com/Hesperyx/"><img align="right" src="https://komarev.com/ghpvc/?username=Hesperyx&label=Views"></a>

<p align="center">
  <span id="dynamic-typing"></span>
</p>

<script>
async function loadHitokoto() {
  try {
    // 获取一言文本
    const res = await fetch('https://v1.hitokoto.cn/?c=f&encode=text');
    const text = await res.text();
    
    // 构造动态打字机 SVG
    const svgUrl = `https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&width=435&lines=${encodeURIComponent(text)}`;
    
    // 插入到页面
    document.getElementById('dynamic-typing').innerHTML = 
      `<a href="https://git.io/typing-svg"><img src="${svgUrl}" alt="Dynamic Typing"></a>`;
  } catch (e) {
    // 失败兜底
    document.getElementById('dynamic-typing').innerHTML = 
      `<a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.demolab.com?font=Fira&pause=1000&width=435&lines=Hello+World" alt="Typing"></a>`;
  }
}
loadHitokoto();
</script>

<table align="center">
    <tr>
        <td align="center">
          <picture>
            <img src="./profile/stats.svg">
          </picture>
        </td>
        <td align="center">
          <picture>
            <img src="./profile/top-langs.svg">
          </picture>
        </td>
    </tr>
</table>

### Trophy 🏆

<div align="center">
  <img src="./profile/trophy.svg"/>
</div>

### contributions

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./dist/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="./dist/github-snake.svg" />
  <img alt="github-snake" src="./dist/github-snake.svg" />
</picture>
