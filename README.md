# CapstoneSA

<p>A real-time dynamic pricing simulation for urban parking spaces using **Python**, **Pandas**, **Numpy**, **Pathway**, and **Bokeh**.  
It adjusts parking prices based on demand, occupancy, traffic conditions, queue lengths, and real-time events, with smooth and explainable pricing changes.</p>
<h3> Techstacks used </h3> 
<table>
  <thead>
    <tr>
      <th>Category</th>
      <th>Technology</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Language</td>
      <td>Python 3.12</td>
    </tr>
    <tr>
      <td>Data Processing</td>
      <td>Pandas, Numpy</td>
    </tr>
    <tr>
      <td>Streaming Engine</td>
      <td>Pathway</td>
    </tr>
    <tr>
      <td>Visualization</td>
      <td>Bokeh</td>
    </tr>
    <tr>
      <td>Environment</td>
      <td>Google Colab</td>
    </tr>
    <tr>
      <td>Version Control</td>
      <td>Git, GitHub</td>
    </tr>
  </tbody>
</table>
<h3>Architecture Flow</h3>

<ol>
  <li><strong> Data Ingestion</strong><br>
    <ul>
      <li>Streaming CSVs with columns: occupancy, capacity, queue length, traffic, special day indicators</li>
      <li>Powered by Pathway</li>
    </ul>
  </li>
  <li><strong> Preprocessing</strong><br>
    <ul>
      <li>Clean string values</li>
      <li>Map traffic conditions to numeric scores</li>
      <li>Normalize demand features</li>
    </ul>
  </li>
  <li><strong> Pricing Models</strong><br>
    <ul>
      <li><strong>Baseline:</strong> Linear price based on occupancy</li>
      <li><strong>Demand-Based:</strong> Adjusted by queue, traffic, and special day indicators</li>
      <li><strong>Competitive:</strong> Incorporates competitor pricing and proximity</li>
    </ul>
  </li>
  <li><strong> Dynamic Simulation</strong><br>
    <ul>
      <li>Prices updated in real-time</li>
      <li>Bounded by minimum and maximum limits</li>
    </ul>
  </li>
  <li><strong> Visualization</strong><br>
    <ul>
      <li>Real-time Bokeh charts for each parking space</li>
    </ul>
  </li>
</ol>

---
<h3>Architecture Diagram</h3>

<pre>
Parking CSV -> Pathway Engine -> Preprocessing + Pricing Logic -> Bokeh Visuals
</pre>
