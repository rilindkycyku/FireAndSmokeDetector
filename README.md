<h1 style="color: #e63946; text-align: center;">Smoke and Flame Detector - Arduino System</h1>

<p style="font-size: 1.2em; text-align: center; color: #444;">
  <strong>Projekt i zhvilluar në kuadër të lëndës Inxhinieri e Sistemeve Kompjuterike në UBT</strong>
</p>

<p style="text-align: center;">
  <strong>Studentët:</strong> Rilind Kyçyku & Ilire Jezerci<br>
  <strong>Ligjëruesi:</strong> Dr. Sc. Luan Mulaku
</p>

<hr style="border: 1px solid #e63946; margin: 2em 0;">

<h2 style="color: #1d3557; border-bottom: 2px solid #e63946; padding-bottom: 0.4em;">Përmbledhja e Projektit</h2>
<p>
  Një sistem sigurie me precizion të lartë i bazuar në <strong>Arduino Uno</strong>, i projektuar për të detektuar zjarrin dhe gazet e rrezikshme në kohë reale. 
  Ky projekt demonstron integrimin e avancuar të sensorëve dhe logjikën e reagimit ndaj rreziqeve në kohë reale për monitorimin e sigurisë.
</p>

<h2 style="color: #1d3557;">Karakteristikat Kryesore</h2>
<ul style="line-height: 1.6;">
  <li><strong>Monitorimi në Kohë Reale:</strong> Lexim i vazhdueshëm i sensorëve MQ-2 (Gaz) dhe IR (Flakë).</li>
  <li><strong>Kanale Alarmi të Pavarura:</strong> LED dhe zhurmues (buzzer) të ndarë për Gazin dhe Flakën për të identifikuar menjëherë llojin e rrezikut.</li>
  <li><strong>Alarmim me Dy Faza:</strong> Alarme zanore me frekuencë të lartë (9000Hz) duke përdorur funksionin <code>tone()</code>.</li>
  <li><strong>Logjika e Bazuar në Kushte:</strong>
    <ul>
      <li><strong>Vetëm Gaz:</strong> Aktivizon LED-in e Kuq 1 dhe Zhurmuesin 1.</li>
      <li><strong>Vetëm Flakë:</strong> Aktivizon LED-in e Kuq 2 dhe Zhurmuesin 2.</li>
      <li><strong>Rrezik i Plotë:</strong> Aktivizimi i të gjitha sistemeve të alarmit.</li>
      <li><strong>Gjendja e Sigurt:</strong> LED-i i Gjelbër aktiv, sistemet e alarmit të fikura.</li>
    </ul>
  </li>
</ul>

<h2 style="color: #1d3557;">Konfigurimi i Pinave</h2>
<table style="width: 100%; border-collapse: collapse; margin: 1em 0; background: #f1f1f1;">
  <tr style="background: #1d3557; color: white;">
    <th style="padding: 10px; border: 1px solid #ddd;">Pina</th>
    <th style="padding: 10px; border: 1px solid #ddd;">Komponenti</th>
  </tr>
  <tr>
    <td style="padding: 10px; border: 1px solid #ddd;">Analog A0</td>
    <td style="padding: 10px; border: 1px solid #ddd;">Sensori i Gazit MQ-2</td>
  </tr>
  <tr>
    <td style="padding: 10px; border: 1px solid #ddd;">Digital 2</td>
    <td style="padding: 10px; border: 1px solid #ddd;">Sensori i Flakës IR</td>
  </tr>
  <tr>
    <td style="padding: 10px; border: 1px solid #ddd;">Digital 3</td>
    <td style="padding: 10px; border: 1px solid #ddd;">LED i Kuq 1 (Paralajmërim Gazi)</td>
  </tr>
  <tr>
    <td style="padding: 10px; border: 1px solid #ddd;">Digital 4</td>
    <td style="padding: 10px; border: 1px solid #ddd;">LED i Kuq 2 (Paralajmërim Flake)</td>
  </tr>
  <tr>
    <td style="padding: 10px; border: 1px solid #ddd;">Digital 6</td>
    <td style="padding: 10px; border: 1px solid #ddd;">Zhurmuesi 2 (Audio për Flakën)</td>
  </tr>
  <tr>
    <td style="padding: 10px; border: 1px solid #ddd;">Digital 7</td>
    <td style="padding: 10px; border: 1px solid #ddd;">Zhurmuesi 1 (Audio për Gazin)</td>
  </tr>
  <tr>
    <td style="padding: 10px; border: 1px solid #ddd;">Digital 8</td>
    <td style="padding: 10px; border: 1px solid #ddd;">LED i Gjelbër (Sistemi OK)</td>
  </tr>
</table>

<h2 style="color: #1d3557;">Kërkesat Harduerike</h2>
<ul style="line-height: 1.6;">
  <li>Arduino Uno</li>
  <li>Moduli i Sensorit të Gazit MQ-2</li>
  <li>Moduli i Sensorit të Flakës IR</li>
  <li>2x Zhurmues Aktivë (Active Buzzers)</li>
  <li>3x LED (Kuq, Kuq, Gjelbër)</li>
  <li>Furnizim me Energji 9V DC</li>
</ul>

<hr style="border: 0; border-top: 1px solid #ddd; margin: 2em 0;">
<p style="text-align: center; color: #888;">
  © 2026 <strong>Rilind Kyçyku</strong> & <strong>Ilire Jezerci</strong> | UBT University
</p>
