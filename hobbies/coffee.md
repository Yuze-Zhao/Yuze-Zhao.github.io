---
layout: page
permalink: /hobbies/coffee/index.html
title: Pour-over Coffee Lab
description: A V60 and light-roast pour-over coffee learning guide with a brew-ratio calculator.
hobbies_section: true
hobby_key: coffee
---

{% include hobby-nav.html %}

<div class="coffee-lab">
  <header class="coffee-header">
    <p class="hobby-kicker">Hobbies · Coffee</p>
    <h1>☕ 手冲咖啡学习指南</h1>
    <p>V60 滤杯 &amp; 浅烘咖啡豆专项</p>
  </header>

  <div class="coffee-grid">
    <section class="coffee-card" tabindex="0" data-tip="如果感觉太淡，尝试调细研磨度；如果感觉太苦，尝试调粗研磨度或降低水温。">
      <h2>📍 冲煮四要素</h2>
      <ul>
        <li><strong>粉水比：</strong>建议 1:15 到 1:17</li>
        <li><strong>研磨度：</strong>中细研磨（类似细盐）</li>
        <li><strong>水温：</strong>90.5℃–96℃</li>
        <li><strong>时间：</strong>总时长约 3:30 分钟</li>
      </ul>
      <p class="coffee-tip">💡 如果感觉太淡，尝试调细研磨度；如果感觉太苦，尝试调粗研磨度或降低水温。</p>
    </section>

    <section class="coffee-card" tabindex="0">
      <h2>🌱 浅烘豆风味库</h2>
      <ul>
        <li><strong>瑰夏：</strong>佛手柑、浆果、蜂蜜</li>
        <li><strong>卡杜拉：</strong>柠檬酸、明亮酸质</li>
        <li><strong>埃塞种：</strong>浓郁花香、热带水果</li>
      </ul>
      <p class="coffee-tip">💡 浅烘豆通常密度较高，注水速度可以稍微放缓，以保证充分萃取。</p>
    </section>

    <section class="coffee-calculator" aria-labelledby="calculator-title">
      <h2 id="calculator-title">⚖️ 粉水比计算器</h2>
      <div class="coffee-calculator-fields">
        <label>咖啡粉重 (g)<input type="number" id="grounds" value="20" min="1" step="0.1" inputmode="decimal"></label>
        <label>目标比例 1 :<input type="number" id="ratio" value="16" min="1" step="0.1" inputmode="decimal"></label>
        <button type="button" id="calculate-water">计算水量</button>
        <output for="grounds ratio" aria-live="polite">需注入：<strong id="water-result">320.0</strong> g</output>
      </div>
    </section>

    <section class="coffee-card coffee-process">
      <h2>🏁 V60 冲煮流程</h2>
      <ol>
        <li><span>1</span><p>润湿滤纸，预热分享壶，放入咖啡粉并归零秤。</p></li>
        <li><span>2</span><p><strong>闷蒸：</strong>注入粉重 2 倍的水，等待 30–45 秒，观察气泡。</p></li>
        <li><span>3</span><p><strong>注水：</strong>从中心画圈，分段注水，保持水位稳定，避免冲淋杯壁。</p></li>
      </ol>
    </section>

    <section class="coffee-mindmap" aria-labelledby="mindmap-title">
      <h2 id="mindmap-title">🗺️ 手冲知识脑图预览</h2>
      <div class="coffee-mindmap-canvas">
        <pre class="mermaid">
mindmap
  root((V60手冲咖啡体系))
    核心器具
      V60特性
      分享壶
      电子秤
      手冲壶
    浅烘豆
      瑰夏
      卡杜拉
      埃塞种
    冲煮变量
      粉水比 1:15–1:17
      中细研磨
      水温 90.5–96℃
    关键技术
      润湿滤纸
      30–45秒闷蒸
      中心画圈
    纠错
      太酸：调细或升温
      太苦：调粗或降温
        </pre>
      </div>
    </section>
  </div>

  <p class="coffee-source">知识来源于《手工咖啡》指南 | 由 NotebookLM 协作生成</p>
</div>

<script>
(function () {
  var grounds = document.getElementById('grounds');
  var ratio = document.getElementById('ratio');
  var result = document.getElementById('water-result');
  var button = document.getElementById('calculate-water');

  function calculateWater() {
    var groundsValue = Number(grounds.value);
    var ratioValue = Number(ratio.value);
    result.textContent = groundsValue > 0 && ratioValue > 0
      ? (groundsValue * ratioValue).toFixed(1)
      : '—';
  }

  button.addEventListener('click', calculateWater);
  grounds.addEventListener('input', calculateWater);
  ratio.addEventListener('input', calculateWater);
}());
</script>

<script type="module">
  import mermaid from 'https://cdn.jsdelivr.net/npm/mermaid@11.16.0/dist/mermaid.esm.min.mjs';

  mermaid.initialize({
    startOnLoad: true,
    theme: 'neutral',
    securityLevel: 'strict',
    mindmap: { padding: 18 }
  });
</script>
