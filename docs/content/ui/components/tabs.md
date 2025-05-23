---
title: Tabs
summary: Tabs allow users to alternate between equally important views within the same context. By dividing content into meaningful sections, they improve its organization and make it easy for users to navigate.
bootstrapLink: components/navs/
description: Organize content with interactive tabs.
---

## Default markup

Use tabs to let users access different sections within one context quickly and with ease. In the default design, the current tab is highlighted, which makes the interface clear and user-friendly.

{% capture html -%}
<div class="card">
  <div class="card-header">
    <ul class="nav nav-tabs card-header-tabs" data-bs-toggle="tabs">
      <li class="nav-item">
        <a href="#tabs-home-ex1" class="nav-link active" data-bs-toggle="tab">Home</a>
      </li>
      <li class="nav-item">
        <a href="#tabs-profile-ex1" class="nav-link" data-bs-toggle="tab">Profile</a>
      </li>
    </ul>
  </div>
  <div class="card-body">
    <div class="tab-content">
      <div class="tab-pane active show" id="tabs-home-ex1">
        <h4>Home tab</h4>
        <div>
          Cursus turpis vestibulum, dui in pharetra vulputate id sed non turpis ultricies fringilla
          at sed facilisis lacus pellentesque purus nibh
        </div>
      </div>
      <div class="tab-pane" id="tabs-profile-ex1">
        <h4>Profile tab</h4>
        <div>
          Fringilla egestas nunc quis tellus diam rhoncus ultricies tristique enim at diam, sem nunc
          amet, pellentesque id egestas velit sed
        </div>
      </div>
    </div>
  </div>
</div>
{%- endcapture %}
{% include "docs/example.html" html=html %}

## Tabs with icons

Add icons to your tab labels, if you want to use a visual element and make the tab content easier to identify.

{% capture html -%}
<div class="card">
  <div class="card-header">
    <ul class="nav nav-tabs card-header-tabs" data-bs-toggle="tabs">
      <li class="nav-item">
        <a href="#tabs-home-ex2" class="nav-link active" data-bs-toggle="tab">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="icon me-2"
            width="24"
            height="24"
            viewBox="0 0 24 24"
            stroke-width="2"
            stroke="currentColor"
            fill="none"
            stroke-linecap="round"
            stroke-linejoin="round"
          >
            <path stroke="none" d="M0 0h24v24H0z" fill="none" />
            <polyline points="5 12 3 12 12 3 21 12 19 12" />
            <path d="M5 12v7a2 2 0 0 0 2 2h10a2 2 0 0 0 2 -2v-7" />
            <path d="M9 21v-6a2 2 0 0 1 2 -2h2a2 2 0 0 1 2 2v6" />
          </svg>
          Home
        </a>
      </li>
      <li class="nav-item">
        <a href="#tabs-profile-ex2" class="nav-link" data-bs-toggle="tab">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="icon me-2"
            width="24"
            height="24"
            viewBox="0 0 24 24"
            stroke-width="2"
            stroke="currentColor"
            fill="none"
            stroke-linecap="round"
            stroke-linejoin="round"
          >
            <path stroke="none" d="M0 0h24v24H0z" fill="none" />
            <circle cx="12" cy="7" r="4" />
            <path d="M6 21v-2a4 4 0 0 1 4 -4h4a4 4 0 0 1 4 4v2" />
          </svg>
          Profile
        </a>
      </li>
      <li class="nav-item ms-auto">
        <a href="#tabs-settings-ex2" class="nav-link" title="Settings" data-bs-toggle="tab">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="icon"
            width="24"
            height="24"
            viewBox="0 0 24 24"
            stroke-width="2"
            stroke="currentColor"
            fill="none"
            stroke-linecap="round"
            stroke-linejoin="round"
          >
            <path stroke="none" d="M0 0h24v24H0z" fill="none" />
            <path
              d="M10.325 4.317c.426 -1.756 2.924 -1.756 3.35 0a1.724 1.724 0 0 0 2.573 1.066c1.543 -.94 3.31 .826 2.37 2.37a1.724 1.724 0 0 0 1.065 2.572c1.756 .426 1.756 2.924 0 3.35a1.724 1.724 0 0 0 -1.066 2.573c.94 1.543 -.826 3.31 -2.37 2.37a1.724 1.724 0 0 0 -2.572 1.065c-.426 1.756 -2.924 1.756 -3.35 0a1.724 1.724 0 0 0 -2.573 -1.066c-1.543 .94 -3.31 -.826 -2.37 -2.37a1.724 1.724 0 0 0 -1.065 -2.572c-1.756 -.426 -1.756 -2.924 0 -3.35a1.724 1.724 0 0 0 1.066 -2.573c-.94 -1.543 .826 -3.31 2.37 -2.37c1 .608 2.296 .07 2.572 -1.065z"
            />
            <circle cx="12" cy="12" r="3" />
          </svg>
        </a>
      </li>
    </ul>
  </div>
  <div class="card-body">
    <div class="tab-content">
      <div class="tab-pane active show" id="tabs-home-ex2">
        <h4>Home tab</h4>
        <div>
          Cursus turpis vestibulum, dui in pharetra vulputate id sed non turpis ultricies fringilla
          at sed facilisis lacus pellentesque purus nibh
        </div>
      </div>
      <div class="tab-pane" id="tabs-profile-ex2">
        <h4>Profile tab</h4>
        <div>
          Fringilla egestas nunc quis tellus diam rhoncus ultricies tristique enim at diam, sem nunc
          amet, pellentesque id egestas velit sed
        </div>
      </div>
      <div class="tab-pane" id="tabs-settings-ex2">
        <h4>Settings tab</h4>
        <div>
          Donec ac vitae diam amet vel leo egestas consequat rhoncus in luctus amet, facilisi sit
          mauris accumsan nibh habitant senectus
        </div>
      </div>
    </div>
  </div>
</div>
{%- endcapture %}
{% include "docs/example.html" html=html %}

## Tabs only with icons

Use tabs without label names to save space and make the tab content easy to recognize for international users.

{% capture html -%}
<div class="card">
  <div class="card-header">
    <ul class="nav nav-tabs card-header-tabs" data-bs-toggle="tabs">
      <li class="nav-item">
        <a href="#tabs-home-ex3" class="nav-link active" data-bs-toggle="tab">
		    {% include "ui/icon.html" icon="home" %}
        </a>
      </li>
      <li class="nav-item">
        <a href="#tabs-profile-ex3" class="nav-link" data-bs-toggle="tab">
          {% include "ui/icon.html" icon="user" %}
        </a>
      </li>
      <li class="nav-item ms-auto">
        <a href="#tabs-settings-ex3" class="nav-link" title="Settings" data-bs-toggle="tab">
          {% include "ui/icon.html" icon="settings" %}
        </a>
      </li>
    </ul>
  </div>
  <div class="card-body">
    <div class="tab-content">
      <div class="tab-pane active show" id="tabs-home-ex3">
        <h4>Home tab</h4>
        <div>
          Cursus turpis vestibulum, dui in pharetra vulputate id sed non turpis ultricies fringilla
          at sed facilisis lacus pellentesque purus nibh
        </div>
      </div>
      <div class="tab-pane" id="tabs-profile-ex3">
        <h4>Profile tab</h4>
        <div>
          Fringilla egestas nunc quis tellus diam rhoncus ultricies tristique enim at diam, sem nunc
          amet, pellentesque id egestas velit sed
        </div>
      </div>
      <div class="tab-pane" id="tabs-settings-ex3">
        <h4>Settings tab</h4>
        <div>
          Donec ac vitae diam amet vel leo egestas consequat rhoncus in luctus amet, facilisi sit
          mauris accumsan nibh habitant senectus
        </div>
      </div>
    </div>
  </div>
</div>
{%- endcapture %}
{% include "docs/example.html" html=html %}

## Tabs with dropdown

Make one or more of your tabs into a dropdown to add more options within one element.

{% capture html -%}
<div class="card">
  <div class="card-header">
    <ul class="nav nav-tabs card-header-tabs" data-bs-toggle="tabs">
      <li class="nav-item">
        <a href="#tabs-home-ex4" class="nav-link active" data-bs-toggle="tab">Home</a>
      </li>
      <li class="nav-item">
        <a href="#tabs-profile-ex4" class="nav-link" data-bs-toggle="tab">Profile</a>
      </li>
      <li class="nav-item dropdown">
        <a
          class="nav-link dropdown-toggle"
          data-bs-toggle="dropdown"
          role="button"
          aria-haspopup="true"
          aria-expanded="false"
          >Dropdown</a
        >
        <div class="dropdown-menu">
          <a class="dropdown-item" href="#"> Action </a>
          <a class="dropdown-item" href="#"> Another action </a>
        </div>
      </li>
    </ul>
  </div>
  <div class="card-body">
    <div class="tab-content">
      <div class="tab-pane active show" id="tabs-home-ex4">
        <h4>Home tab</h4>
        <div>
          Cursus turpis vestibulum, dui in pharetra vulputate id sed non turpis ultricies fringilla
          at sed facilisis lacus pellentesque purus nibh
        </div>
      </div>
      <div class="tab-pane" id="tabs-profile-ex4">
        <h4>Profile tab</h4>
        <div>
          Fringilla egestas nunc quis tellus diam rhoncus ultricies tristique enim at diam, sem nunc
          amet, pellentesque id egestas velit sed
        </div>
      </div>
    </div>
  </div>
</div>
{%- endcapture %}
{% include "docs/example.html" html=html %}

## Full-width tabs

Add the `.nav-fill` class to make the tabs take up the full space of the parent element.

{% capture html -%}
<div class="card">
  <div class="card-header">
    <ul class="nav nav-tabs card-header-tabs nav-fill" data-bs-toggle="tabs">
      <li class="nav-item">
        <a href="#tabs-home-ex5" class="nav-link active" data-bs-toggle="tab">
		  	 {% include "ui/icon.html" icon="home" %}
        </a>
      </li>
      <li class="nav-item">
        <a href="#tabs-profile-ex5" class="nav-link" data-bs-toggle="tab">
		    {% include "ui/icon.html" icon="user" %}
        </a>
      </li>
      <li class="nav-item">
        <a href="#tabs-activity-ex5" class="nav-link" data-bs-toggle="tab">
          {% include "ui/icon.html" icon="activity" %}
        </a>
      </li>
    </ul>
  </div>
  <div class="card-body">
    <div class="tab-content">
      <div class="tab-pane active show" id="tabs-home-ex5">
        <h4>Home tab</h4>
        <div>
          Cursus turpis vestibulum, dui in pharetra vulputate id sed non turpis ultricies fringilla
          at sed facilisis lacus pellentesque purus nibh
        </div>
      </div>
      <div class="tab-pane" id="tabs-profile-ex5">
        <h4>Profile tab</h4>
        <div>
          Fringilla egestas nunc quis tellus diam rhoncus ultricies tristique enim at diam, sem nunc
          amet, pellentesque id egestas velit sed
        </div>
      </div>
      <div class="tab-pane" id="tabs-activity-ex5">
        <h4>Activity tab</h4>
        <div>
          Donec ac vitae diam amet vel leo egestas consequat rhoncus in luctus amet, facilisi sit
          mauris accumsan nibh habitant senectus
        </div>
      </div>
    </div>
  </div>
</div>
{%- endcapture %}
{% include "docs/example.html" html=html %}
