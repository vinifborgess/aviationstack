## ✈️ Aviation Data Engineering Project | Modern Data Engineering E2E Project
Using AviationStack API to obtain historical flight data and perform basic flight data processing and analysis.

## 📖 About
The following project uses the AviationStack API to access aviation data. Each aviationstack account is assigned a unique access key, known as the master key, which must be used to authenticate requests to the API. You can find your master key in your account dashboard. Each account is assigned only one master key.

If you want to view customized data, enter your key, modify the code, and download the project to your local machine.

To connect to the API, simply attach the access_key parameter to any valid API endpoint URL and set it to your master key. See the example below:

```
https://api.aviationstack.com/v1/flights?access_key=YOUR_ACCESS_KEY
```

Replace YOUR_ACCESS_KEY with your actual master key.

## 🚫 Problem Statement:
Obtain historical flight data and perform basic flight data processing and analysis.

## 💾 Launch
[Click to launch the full project here.](https://app.powerbi.com/reportEmbed?reportId=6db999f7-44e4-4c11-a815-7d9da75041cd&autoAuth=true&ctid=461455b5-e6f3-430b-ab4c-9bc4818a4cd3).

## 🎯 Project Roadmap
On this [public board](https://trello.com/invite/b/66b7fcfaf9e28f7e1c9cbba9/ATTI0c932cb843b0cd1656fa350f0ab45ccb4BB32D48/aviation-data-engineering-project-modern-data-engineering-e2e-project), users can see the dev roadmap. The platform also includes future updates and patch notes.

## 📐 Architecture:
This architecture is designed/developed to be a robust and detailed product, standardized, and able to re-usability.

```
                +----------------------------------+
                |          Data Extraction         |
                |----------------------------------|
                | AviationStack API                |
                | Params: access_key, airline_iata |
                +----------------+-----------------+
                                 |
                                 v
                +----------------+-----------------+
                |       Data Transformation        |
                |----------------------------------|
                | Parse JSON, Normalize Fields     |
                |                                 |
                +--------+-----------------+-------+
                         |                 |
                         v                 v
                +--------+--------+ +------+------+
                |   CSV Storage   | | SQLite DB   |
                |-----------------| |-------------|
                | Write to CSV    | | Insert Data |
                +--------+--------+ +------+------+
                         |                 |
                         v                 v
                +--------+-----------------+-------+
                |        Data Retrieval            |
                |----------------------------------|
                | Query SQLite DB, Print Results   |
                +----------------------------------+
```

<h1 align="center">
  <a
    target="_blank"
    href="https://raw.githubusercontent.com/vinifborgess/aviationstack/main/project_architecture.png"
  >
    <img
      align="center"
      alt="Mage"
      src="https://raw.githubusercontent.com/vinifborgess/aviationstack/main/project_architecture.png"
      style="width:100%;"
    />
  </a>
</h1>
<p align="center">

## 🏗️ Built with:
Language: Python;

Softwares: AviationStackAPI, Figma, PowerBI.

## 🕸️ Data Model
Work in progress. Please, come back later.

## 🆕 Patch Notes
Work in progress. Please, come back later.

## 👨🏻 Author
[Vinícius Borges](https://github.com/vinifborgess).

## 👋🏻 Thanks!
<h1 align="center">
  <a
    target="_blank"
    href="https://mage.ai"
  >
    <img
      align="center"
      alt="Mage"
      src="https://gifdb.com/images/high/flying-pixel-plane-clouds-vf6rfbxtsecs16hv.gif"
      style="width:100%;"
    />
  </a>
</h1>
<p align="center">



