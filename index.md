---
layout: page
title: Made with pleasure but serious. A C# cross platform game toolkit to create 2D and 3D games
permalink: /
---

{% if site.showSpotlight == true %}
<div class="row">
    <div class="col-md-2"></div>
    <div class="col-md-8">
        <div class="alert alert-danger" role="alert">
            We are working hard to complete clean and easly understand documentation. <a href="https://www.patreon.com/impression" class="alert-link">Support us at Patreon</a>.
        </div>
    </div>
    <div class="col-md-2"></div>
</div>
{% endif %}

<div class="jumbotron">
    <h2 class="text-center">Impression</h2>
    <p class="text-center"><img src="https://img.shields.io/nuget/v/Impression.Windows.svg"/></p>
    <br>
    <h4 class="text-center">Made with pleasure but serious</h4>
    <h4 class="text-center">A C# cross platform game toolkit to create 2D and 3D games</h4>
    <br>
    <br>
    <p class="text-center">
        <span class="badge badge-feature">Cross Platform</span>
        <span class="badge badge-feature">Free</span>
        <span class="badge badge-feature">Extensible</span>
    </p>
</div>

***

<div class="row">
    <div class="col-md-2 text-center">
        <h5>Android</h5>
        <a href="#">
            <img src="https://img.shields.io/nuget/dt/Impression.Android.svg" />
        </a>
    </div>
    <div class="col-md-2 text-center">
        <h5>iOS</h5>
        <a href="#">
            <img src="https://img.shields.io/nuget/dt/Impression.iOS.svg" />
        </a>
    </div>
    <div class="col-md-2 text-center">
        <h5>Linux</h5>
        <a href="#">
            <img src="https://img.shields.io/nuget/dt/Impression.Linux.svg" />
        </a>
    </div>
    <div class="col-md-2 text-center">
        <h5>Mac</h5>
        <a href="#">
            <img src="https://img.shields.io/nuget/dt/Impression.Mac.svg" />
        </a>
    </div>
    <div class="col-md-2 text-center">
        <h5>Universal Windows</h5>
        <a href="#">
            <img src="https://img.shields.io/nuget/dt/Impression.UniversalWindows.svg" />
        </a>
    </div>
    <div class="col-md-2 text-center">
        <h5>Windows</h5>
        <a href="#">
            <img src="https://img.shields.io/nuget/dt/Impression.Windows.svg" />
        </a>
    </div>
</div>

***

<h4 class="text-center">Prerequisite</h4>
<p class="text-center">You need development toolkit to easily develop game. <br>Currently, it's contains project and content builder. See <a href="/docs/getting-started/installation" target="_blank">more prerequisite installation</a>.</p>
<br>
<p class="text-center">
<a href="#" class="btn btn-default">Windows&nbsp;&nbsp;&nbsp;<span class="glyphicon glyphicon-cloud-download" aria-hidden="true"></span></a>&nbsp;&nbsp;&nbsp;<a href="#" class="btn btn-default">Mac&nbsp;&nbsp;&nbsp;<span class="glyphicon glyphicon-cloud-download" aria-hidden="true"></span></a>&nbsp;&nbsp;&nbsp;<a href="#" class="btn btn-default">Linux&nbsp;&nbsp;&nbsp;<span class="glyphicon glyphicon-cloud-download" aria-hidden="true"></span></a></p>

<br>
<br>
<h4 class="text-center">New Project</h4>
<p class="text-center">Open terminal or command prompt<br>
run <code>{path-to}\ProjectBuilder.exe new YourProjectName</code><br>
If you on Mac or Linux environment<br>
run <code>mono {path-to}\ProjectBuilder.exe new YourProjectName</code>
</p>
<br>
<br>
<h4 class="text-center">Open Project</h4>
<p class="text-center">Double click <code>YourProjectName.sln</code> on <code>YourProjectName</code> directory. <br>
A C# IDE should be open.
</p>
<br>
<br>
<h4 class="text-center">Build and Run</h4>
<p class="text-center">Still in C# IDE, build and run like other C# projects. <br>
These action will download some dependencies, but just for in first time only. <br>
If successfully, an empty <span class="badge badge-feature">burlywood color</span> game window will appear.</p>

<br>
<br>
<h4 class="text-center">Now, It's Your Turn!</h4>
<p class="text-center"><a href="{{ "docs/preface/introduction" | prepend: site.baseurl }}" target="_blank">Read the docs</a>, <a href="https://github.com/impression3d/Impression.Examples" target="_blank">explore the examples</a>, and create your game.</p>
