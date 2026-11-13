<div align="center">

<img src="docs/media/hero.svg" alt="Cinemania — the trending hero, weekly trends and a catalogue search, then a film's details modal adds it to My Library" width="100%">

<p>
  <a href="https://kutluhangil.github.io/Cinemania/"><img alt="Live" src="https://img.shields.io/badge/live-GitHub%20Pages-f87719?style=for-the-badge&labelColor=4a1f14"></a>
  <img alt="TMDB" src="https://img.shields.io/badge/data-TMDB%20API-ff3d3d?style=for-the-badge&labelColor=4a1f14">
  <img alt="Vanilla JS" src="https://img.shields.io/badge/JavaScript-vanilla%20%2B%20Vite-ffc94a?style=for-the-badge&labelColor=4a1f14">
  <img alt="Team" src="https://img.shields.io/badge/GoIT-team%20project-f87719?style=for-the-badge&labelColor=4a1f14">
</p>

<p><em>A responsive movie discovery platform built with vanilla JavaScript on the TMDB API.<br>
Browse trending and upcoming films, search the catalogue and keep your own library.</em></p>

<img src="src/images/readme/desktop_home.png" alt="Cinemania home page on desktop" width="100%">

</div>

<img src="docs/media/divider.svg" width="100%" alt="">

## The idea

Cinemania is what a team of GoIT students built with no framework at all: HTML partials stitched together at build time by Vite, plain JavaScript modules for each section, and the TMDB API for every film, poster and trailer. The result is a three-page site (home, catalogue, my library) that works from a 320 px phone to a wide desktop.

> **Small modules, one owner each.** Every block of the page (hero, weekly trends, upcoming, catalogue, pagination, modals, footer) is its own partial and script, which is how six people could work on it in parallel without stepping on each other.

<img src="docs/media/divider.svg" width="100%" alt="">

## Features

| | |
|---|---|
| **Daily trending hero** | The trending film of the day, front and centre, with its rating and a trailer button. |
| **Weekly trends and upcoming** | This week's trends and this month's releases. |
| **Catalogue** | Keyword search with a year filter, server-side pagination and load more. |
| **Movie modal** | Details (votes, popularity, genres, overview) and the trailer in a modal. |
| **My Library** | Add and remove films, kept in localStorage. |
| **Themes** | Dark and light, remembered between visits. |
| **Team modal** | The footer opens a modal introducing the developers. |
| **Polish** | A global loader, scroll-to-top, retina images, and W3C-valid HTML and CSS. |
| **Mobile first** | Layouts at 320, 768 and 1280 px. |
| **README in four languages** | English here, plus Turkish, Polish and Romanian versions in the repository. |

<table>
  <tr>
    <td width="20%"><img src="src/images/readme/mobile_home.png" alt="Mobile home"></td>
    <td width="40%"><img src="src/images/readme/tablet_catalog.png" alt="Tablet catalogue"></td>
    <td width="40%"><img src="src/images/readme/desktop_library.png" alt="Desktop library"></td>
  </tr>
</table>

<img src="docs/media/divider.svg" width="100%" alt="">

## How it fits together

```mermaid
flowchart LR
  TMDB[TMDB API<br/>trending · search · details · videos] --> API[js/api/movies-api.js]
  API --> HERO[hero] & WEEK[weekly trends] & UP[upcoming] & CAT[catalogue · pagination]
  CAT --> MOD[movie modal · trailer]
  MOD --> LIB[(My Library<br/>localStorage)]
  P[HTML partials] --> VITE[Vite build]
```

<img src="docs/media/divider.svg" width="100%" alt="">

## My part

I built the footer and the team modal, and kept the team section of this README up to date with roles and links.

<img src="docs/media/divider.svg" width="100%" alt="">

## Türkçe özet

**Cinemania**, TMDB API üzerinde vanilla JavaScript ile ekip olarak geliştirdiğimiz duyarlı bir film keşif platformu. Günün trend filmi, haftalık trendler, bu ayın vizyondakileri, yıl filtreli katalog araması, fragmanlı film detayı ve kişisel kütüphane içeriyor; karanlık ve aydınlık tema var. GoIT Full Stack programında grup projesi olarak hazırlandı; footer ve ekip modalı benim sorumluluğumdaydı. Türkçe, Lehçe ve Rumence README'ler depoda ayrıca duruyor.

<img src="docs/media/divider.svg" width="100%" alt="">

<h2 id="team-members">👥 Geliştirici Ekip & Sorumluluklar</h2>

<ul>
  <li>
    <strong>Çiğdem Ergal</strong> — Team Lead<br />
    <em>Sorumluluk:</em> Header & Liderlik<br />
    <a href="https://github.com/CigdemErgal" target="_blank">
      <img src="src/images/readme/github-icon.svg" alt="GitHub" width="18" />
    </a>
    <a href="https://www.linkedin.com/in/%C3%A7i%C4%9Fdem-ergal/" target="_blank">
      <img src="src/images/readme/linkedin-icon.svg" alt="LinkedIn" width="18" />
    </a>
  </li>

  <li>
    <strong>Halenur Gürel</strong> — Scrum Master<br />
    <em>Sorumluluk:</em> Hero & Scrum Yönetimi<br />
    <a href="https://github.com/halenurgurel" target="_blank">
      <img src="src/images/readme/github-icon.svg" alt="GitHub" width="18" />
    </a>
    <a href="https://www.linkedin.com/in/halenurgurel/" target="_blank">
      <img src="src/images/readme/linkedin-icon.svg" alt="LinkedIn" width="18" />
    </a>
  </li>

  <li>
    <strong>Ali Hamza Çakmak</strong> — Developer<br />
    <em>Sorumluluk:</em> Modals (Detail & Trailer)<br />
    <a href="https://github.com/MRMARUL" target="_blank">
      <img src="src/images/readme/github-icon.svg" alt="GitHub" width="18" />
    </a>
    <a href="https://www.linkedin.com/in/ali-hamza-%C3%A7akmak-8112553a8/" target="_blank">
      <img src="src/images/readme/linkedin-icon.svg" alt="LinkedIn" width="18" />
    </a>
  </li>

  <li>
    <strong>Aslıhan Erdal</strong> — Developer<br />
    <em>Sorumluluk:</em> Upcoming This Month<br />
    <a href="https://github.com/ERDLL0" target="_blank">
      <img src="src/images/readme/github-icon.svg" alt="GitHub" width="18" />
    </a>
    <a href="https://www.linkedin.com/in/aslihan-erdal/" target="_blank">
      <img src="src/images/readme/linkedin-icon.svg" alt="LinkedIn" width="18" />
    </a>
  </li>

  <li>
    <strong>Burak Gökay</strong> — Developer<br />
    <em>Sorumluluk:</em> Weekly Trends<br />
    <a href="https://github.com/bgokay007-tech" target="_blank">
      <img src="src/images/readme/github-icon.svg" alt="GitHub" width="18" />
    </a>
    <a href="https://www.linkedin.com/in/burak-g%C3%B6kay-196b66348/" target="_blank">
      <img src="src/images/readme/linkedin-icon.svg" alt="LinkedIn" width="18" />
    </a>
  </li>

  <li>
    <strong>Kerem Yıldırım</strong> — Developer<br />
    <em>Sorumluluk:</em> Catalog<br />
    <a href="https://github.com/keremyldrm61" target="_blank">
      <img src="src/images/readme/github-icon.svg" alt="GitHub" width="18" />
    </a>
    <a href="https://www.linkedin.com/in/kerem-y%C4%B1ld%C4%B1r%C4%B1m-0053a5191/" target="_blank">
      <img src="src/images/readme/linkedin-icon.svg" alt="LinkedIn" width="18" />
    </a>
  </li>

  <li>
    <strong>Yusuf Soylu</strong> — Developer<br />
    <em>Sorumluluk:</em> Pagination<br />
    <a href="https://github.com/soylu1092" target="_blank">
      <img src="src/images/readme/github-icon.svg" alt="GitHub" width="18" />
    </a>
    <a href="https://www.linkedin.com/in/yusuf-soylu-525236306/" target="_blank">
      <img src="src/images/readme/linkedin-icon.svg" alt="LinkedIn" width="18" />
    </a>
  </li>

  <li>
    <strong>Nur Seda Ağgünlü</strong> — Developer<br />
    <em>Sorumluluk:</em> My Library<br />
    <a href="https://github.com/nursedaaggunlu" target="_blank">
      <img src="src/images/readme/github-icon.svg" alt="GitHub" width="18" />
    </a>
    <a href="https://www.linkedin.com/in/nur-seda-aggunlu/" target="_blank">
      <img src="src/images/readme/linkedin-icon.svg" alt="LinkedIn" width="18" />
    </a>
  </li>

  <li>
    <strong>Zehra Yazıcı</strong> — Developer<br />
    <em>Sorumluluk:</em> My Library Hero<br />
    <a href="https://github.com/zehrayazici" target="_blank">
      <img src="src/images/readme/github-icon.svg" alt="GitHub" width="18" />
    </a>
    <a href="https://www.linkedin.com/in/zehrayazici/" target="_blank">
      <img src="src/images/readme/linkedin-icon.svg" alt="LinkedIn" width="18" />
    </a>
  </li>

  <li>
    <strong>Kutluhan Gül</strong> — Developer<br />
    <em>Sorumluluk:</em> Footer & Team Modal<br />
    <a href="https://github.com/kutluhangil" target="_blank">
      <img src="src/images/readme/github-icon.svg" alt="GitHub" width="18" />
    </a>
    <a href="https://www.linkedin.com/in/kutluhangil/" target="_blank">
      <img src="src/images/readme/linkedin-icon.svg" alt="LinkedIn" width="18" />
    </a>
  </li>
</ul>

<img src="docs/media/divider.svg" width="100%" alt="">

## Development

```sh
npm install
npm run dev      # http://localhost:5173
npm run build
```

```
src/index.html · page-2.html · my-library.html   the three pages
src/partials/   header, hero, weekly trends, upcoming, catalogue, pagination, modals, footer
src/js/         one module per section, plus api/movies-api.js
src/css/        styles per section
```

<div align="center">
<br>
<a href="https://github.com/kutluhangil"><img src="docs/media/signature.svg" width="100%" alt="Team project, contribution by kutluhangil"></a>
<sub>Fork of <a href="https://github.com/january-javaScript-project/cinemania">january-javaScript-project/cinemania</a> · created for educational purposes in the GoIT Full Stack programme · data from TMDB · films in the banner are invented.</sub>
</div>
