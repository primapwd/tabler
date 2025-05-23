---
title: Page headers
summary: Page heading examples for Tabler
description: Examples of Tabler page headers.
---

## Simple header

{% capture html -%}
<div class="page-header">
  <div class="row align-items-center">
    <div class="col">
      <div class="page-pretitle">Overview</div>
      <h2 class="page-title">Dashboard</h2>
    </div>
    <div class="col-auto ms-auto">
      <div class="btn-list">
        <span class="d-none d-sm-inline">
          <a href="#" class="btn"> New view </a>
        </span>
        <a
          href="#"
          class="btn btn-primary d-none d-sm-inline-block"
          data-bs-toggle="modal"
          data-bs-target="#modal-report"
        >
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
            <line x1="12" y1="5" x2="12" y2="19" />
            <line x1="5" y1="12" x2="19" y2="12" />
          </svg>
          Create new report
        </a>
        <a
          href="#"
          class="btn btn-primary d-sm-none btn-icon"
          data-bs-toggle="modal"
          data-bs-target="#modal-report"
          aria-label="Create new report"
        >
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
            <line x1="12" y1="5" x2="12" y2="19" />
            <line x1="5" y1="12" x2="19" y2="12" />
          </svg>
        </a>
      </div>
    </div>
  </div>
</div>
{%- endcapture %}
{% include "docs/example.html" html=html %}

## With meta, avatar and actions

{% capture html -%}
<div class="page-header">
  <div class="row align-items-center">
    <div class="col-auto">
      <span
        class="avatar avatar-md"
        style="background-image: url(/static/avatars/023m.jpg)"
      ></span>
    </div>
    <div class="col">
      <h2 class="page-title">Paweł Kuna</h2>
      <div class="page-subtitle">
        <div class="row">
          <div class="col-auto">
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
              <line x1="3" y1="21" x2="21" y2="21" />
              <path d="M5 21v-14l8 -4v18" />
              <path d="M19 21v-10l-6 -4" />
              <line x1="9" y1="9" x2="9" y2="9.01" />
              <line x1="9" y1="12" x2="9" y2="12.01" />
              <line x1="9" y1="15" x2="9" y2="15.01" />
              <line x1="9" y1="18" x2="9" y2="18.01" />
            </svg>
            <a href="#" class="text-reset">UI Designer at Tabler</a>
          </div>
          <div class="col-auto">
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
              <circle cx="9" cy="7" r="4" />
              <path d="M3 21v-2a4 4 0 0 1 4 -4h4a4 4 0 0 1 4 4v2" />
              <path d="M16 3.13a4 4 0 0 1 0 7.75" />
              <path d="M21 21v-2a4 4 0 0 0 -3 -3.85" />
            </svg>
            <a href="#" class="text-reset">194 friends</a>
          </div>
          <div class="col-auto text-success">
            {% include "ui/icon.html" icon="check" %}
            Verified
          </div>
        </div>
      </div>
    </div>
    <div class="col-auto d-none d-md-flex">
      <a href="#" class="btn btn-primary">
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
          <path d="M4 21v-13a3 3 0 0 1 3 -3h10a3 3 0 0 1 3 3v6a3 3 0 0 1 -3 3h-9l-4 4" />
          <line x1="8" y1="9" x2="16" y2="9" />
          <line x1="8" y1="13" x2="14" y2="13" />
        </svg>
        Send message
      </a>
    </div>
  </div>
</div>
{%- endcapture %}
{% include "docs/example.html" html=html %}

## With meta, search and actions

{% capture html -%}
<div class="page-header">
  <div class="row align-items-center">
    <div class="col">
      <h2 class="page-title">Gallery</h2>
      <div class="text-secondary mt-1">1-12 of 241 photos</div>
    </div>
    <div class="col-auto ms-auto d-print-none">
      <div class="d-flex">
        <div class="me-3 d-none d-md-block">
          <div class="input-icon">
            <input type="text" class="form-control" placeholder="Search…" />
            <span class="input-icon-addon">
              {% include "ui/icon.html" icon="search" %}
            </span>
          </div>
        </div>
        <a href="#" class="btn btn-primary">
          {% include "ui/icon.html" icon="plus" %}
          Add photo
        </a>
      </div>
    </div>
  </div>
</div>
{%- endcapture %}
{% include "docs/example.html" html=html %}

## Bordered header

A page header with a border to separate content is an effective way to organize and present information in a clear and visually appealing way.

{% capture html -%}
<div class="page-header page-header-border">
  <div class="container-fluid">
    <div class="row align-items-center">
      <div class="col">
        <h2 class="page-title">Improve cards with no border</h2>
        <div class="text-secondary mt-1">
          <a href="#" class="text-reset">#693</a>
          opened by <a href="#" class="text-body">Jeffie Lewzey</a> in
          <a href="#" class="text-body">Calendar Page</a>
        </div>
      </div>
      <div class="col-auto">
        <div class="btn-list">
          <a href="#" class="btn">
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
              <path d="M7 7h-1a2 2 0 0 0 -2 2v9a2 2 0 0 0 2 2h9a2 2 0 0 0 2 -2v-1" />
              <path d="M20.385 6.585a2.1 2.1 0 0 0 -2.97 -2.97l-8.415 8.385v3h3l8.385 -8.415z" />
              <path d="M16 5l3 3" />
            </svg>
            Edit
          </a>
          <a href="#" class="btn d-none d-md-inline-flex">
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
                d="M10 5a2 2 0 0 1 4 0a7 7 0 0 1 4 6v3a4 4 0 0 0 2 3h-16a4 4 0 0 0 2 -3v-3a7 7 0 0 1 4 -6"
              />
              <path d="M9 17v1a3 3 0 0 0 6 0v-1" />
            </svg>
            Subscribe
          </a>
        </div>
      </div>
    </div>
  </div>
</div>
{%- endcapture %}
{% include "docs/example.html" html=html %}

## Header with breadcrumb and actions

A page header with breadcrumb and actions is a common design element found in many websites and applications. The header typically appears at the top of the page and includes a breadcrumb trail, which shows the user the path they have taken to reach the current page. The breadcrumb can be clickable, allowing the user to navigate back to previous pages.

In addition to the breadcrumb, the header often includes actions or buttons that allow the user to perform common tasks related to the current page. These actions may include things like adding a new item, editing existing content, or deleting items.

{% capture html -%}
<div class="page-header">
  <div class="row align-items-center mw-100">
    <div class="col">
      <div class="mb-1">
        <ol class="breadcrumb" aria-label="breadcrumbs">
          <li class="breadcrumb-item">
            <a href="#">Home</a>
          </li>
          <li class="breadcrumb-item">
            <a href="#">Library</a>
          </li>
          <li class="breadcrumb-item active" aria-current="page">
            <a href="#">Articles</a>
          </li>
        </ol>
      </div>
      <h2 class="page-title">
        <span class="text-truncate"
          >Knights of Ni, we are but simple travelers who seek the enchanter who lives beyond these
          woods.</span
        >
      </h2>
    </div>
    <div class="col-auto">
      <div class="btn-list">
        <a href="#" class="btn d-none d-md-inline-flex">
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
            <path d="M7 7h-1a2 2 0 0 0 -2 2v9a2 2 0 0 0 2 2h9a2 2 0 0 0 2 -2v-1" />
            <path d="M20.385 6.585a2.1 2.1 0 0 0 -2.97 -2.97l-8.415 8.385v3h3l8.385 -8.415z" />
            <path d="M16 5l3 3" />
          </svg>
          Edit
        </a>
        <a href="#" class="btn btn-primary"> Publish </a>
      </div>
    </div>
  </div>
</div>
{%- endcapture %}
{% include "docs/example.html" html=html %}

