---
title: Home
layout: default.html
---

<article>
  <h2>Regulamentação</h2>
  <ul>
  {%- for placa in placas.R -%}
    <li>
      <figure>
        <figcaption>
          <h3>R-{{ placa.id }}</h3>
          <p>{{ placa.name }}</p>
        </figcaption>
        <img src="placas/R{{ placa.file }}.jpg">
      </figure>
    </li>
  {%- endfor -%}
  </ul>
  <hr>
  <ul>
  {%- for placa in placas.R_total -%}
    <li>
      <figure class="faltante">
        <figcaption>
          <h3>R-{{ placa }}</h3>
        </figcaption>
        <img src="placas/falta/R{{ placa }}.png">
      </figure>
    </li>
  {%- endfor -%}
  </ul>
</article>
<article>
  <h2>Advertência</h2>
  <ul>
  {%- for placa in placas.A -%}
    <li>
      <figure>
        <figcaption>
          <h3>A-{{ placa.id }}</h3>
          <p>{{ placa.name }}</p>
        </figcaption>
        <img src="placas/A{{ placa.file }}.jpg">
      </figure>
    </li>
  {%- endfor -%}
  </ul>
  <hr>
  <ul>
  {%- for placa in placas.A_total -%}
    <li>
      <figure class="faltante">
        <figcaption>
          <h3>A-{{ placa }}</h3>
        </figcaption>
        <img src="placas/falta/A{{ placa }}.png">
      </figure>
    </li>
  {%- endfor -%}
  </ul>
</article>