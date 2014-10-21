---
layout: base 
---

<section id="schedule">
    <div class="container">
        <div class="page-header">
        <h2>Hackathon Schedule</h2>
        <h3>Saturday, 25 October 2014</h3>
    </div>

<table class="table">
    <tbody>
        <tr>
            <th>Time</th>
            <th>Event</th>
        </tr>
        <tr >
            <td>8:00 AM</td>
            <td>Doors Open for Hackathon Participants and Volunteers</td>
        </tr>
        <tr class="info">
            <td>8:00 AM</td>
            <td>Breakfast Served</td>
        </tr>
        <tr class="success">
            <td>8:30 AM</td>
            <td>Air Force Background Presentation</td>
        </tr>
        <tr>
            <td>9:00 AM</td>
            <td>Team Formation</td>
        </tr>
        <tr>
            <td>10:00 AM</td>
            <td>Let the Hacking Begin!</td>
        </tr>
        <tr class="warning">
            <td>12:00 PM</td>
            <td>Day Pass Starts</td>
        </tr>
        <tr class="info">
            <td>12:00 PM</td>
            <td>Lunch Served</td>
        </tr>
        <tr class="success">
            <td>12:30 PM</td>
        <td>OpenBCI: <a href="#openbci">An Open-Source Brain-Computer Interface</a></td>
        </tr>   
        <tr class="success">
            <td>12:45 PM</td>
            <td>OpenBCI: Hands-On Workshop on OpenBCI hardware</td>
        </tr>
        <tr class="success">
            <td>1:30 PM</td>
            <td>Plot.ly: <a href="#plotly">Sensor Data Visualization</a></td>
        </tr>
        <tr class="success">
            <td>1:45 PM</td>
            <td>Plot.ly: <a href="https://plot.ly/workshop/">Hands-On Workshop using sensors and Plot.ly</a></td>
        </tr>
        <tr class="success">
            <td>2:30 PM</td>
            <td>Strap: Why Analytics Matter</td>
        </tr>
        <tr class="success">
            <td>2:45 PM</td>
            <td>Strap: Hands-On Workshop with Pebble and Strap</td>
        </tr>
        <tr class="success">
            <td>3:30 PM</td>
            <td>Github: <a href="#github_flow">The Github Flow</a></td>
        </tr>

        <tr class="success">
            <td>4:30 PM</td>
            <td>Tenet3: <a href="#tenet3_prez">Visualizing Data with D3.js</a></td>
        </tr>
        <tr class="success">
            <td>4:45 PM</td>
            <td>Tenet3: Q&A</td>
        </tr>
        <tr class="info">
            <td>5:30 PM</td>
            <td>Dinner Served</td>
        </tr>
        <tr class="success">
            <td>6:00 PM</td>
            <td>Redwall: <a href="#redwall_prez">Mobile device sensors - data mining and visualization implications</a></td>
        </tr>
        <tr class="success">
            <td>6:15 PM</td>
            <td>Redwall: Q&A</td>
        </tr>
        <tr>
            <td>7:00 PM</td>
            <td>Socializing / Unconference </td>
        </tr>
        <tr class="warning">
            <td>10:30 PM</td>
            <td>Day Pass Ends</td>
        </tr>
        <tr class="info">
            <td>11:00 PM</td>
            <td>Late Night Snack Served</td>
        </tr>
    </tbody>
</table>

<p> 
<div style="color: blue;">HACK-THROUGH-THE-NIGHT</div>
</p>

<h3>Sunday, 26 October 2014</h3>
<table class="table">
    <tbody>
        <tr>
            <th>Time</th>
            <th>Event</th>
        </tr>
        <tr class="info">
            <td>8:00 AM</td>
            <td>Breakfast served</td>
        </tr>
        <tr>
            <td>10:00 AM</td>
            <td>Presentation Tech Check / Practice</td>
        </tr>
        <tr class="info">
            <td>12:00 PM</td>
            <td>Lunch Served</td>
        </tr>
        <tr>
            <td>1:45 PM</td>
            <td>Project Submission Deadline</td>
        </tr>
        <tr>
            <td>2:00 PM</td>
            <td>Team Presentations and Judging</td>
        </tr>
        <tr class="info">
            <td>3:45 PM</td>
            <td>Appetizers Served</td>
        </tr>
        <tr>
            <td>4:30 PM</td>
            <td>Prizes and Awards</td>
        </tr>
    </tbody>
</table>
</div>
</section>
<section id="presentations">
<div class="container">

<h2>Presentations and Workshops</h2>

{% for presentation in site.data.presentations %}
<div class="presentation-title row">
<div class="col-xs-12 col-sm-8">
<h3 id="{{presentation.id}}">{{presentation.title}}</h3>
</div>
<div class="col-xs-12 col-sm-4">
{% for presenter in presentation.presenters %}
<div class="presenter pull-right">
    <img src="{{ presenter.photo | asset_path }}"  class="img-rounded" title="{{presenter.name}}" alt="{{presenter.name}}" />
</div>
{% endfor %}
</div>
</div><!-- End Presentation Title Row -->
<div class="presentation-content row">
<p>
{{presentation.summary}}
</p>
</div><!-- End Row -->
{% endfor %}

</section>