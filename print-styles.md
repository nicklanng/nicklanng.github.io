<style>
@media print {
  @page {
    size: A4;
    margin-top: 18mm;
    margin-right: 18mm;
    margin-bottom: 18mm;
    margin-left: 18mm;
  }

  :root {
    color-scheme: dark !important;
    --color-bg-1: #0c1017;
    --color-bg-2: #0f1419;
    --color-fg-1: #cbd5e1;
    --color-fg-2: #f1f5f9;
    --color-fg-3: #64748b;
    --color-fg-4: #475569;
    --color-fg-5: #334155;
    --color-accent: #14b8a6;
  }

  html {
    font-size: 12px !important;
    -webkit-print-color-adjust: exact !important;
    print-color-adjust: exact !important;
  }

  body,
  .content,
  .content__inner,
  .content h1,
  .content h2,
  .content h3,
  .content h4,
  .content h5,
  .content p,
  .content li,
  .content strong,
  .content a:not(.header-link),
  .content code,
  table,
  th,
  td {
    -webkit-print-color-adjust: exact !important;
    print-color-adjust: exact !important;
  }

  .top-bar,
  .menu,
  .header-link,
  .content__inner > style {
    display: none !important;
  }

  .content {
    margin: 0 !important;
    padding: 0 !important;
    overflow: visible !important;
    isolation: auto !important;
  }

  .content__inner {
    max-width: none !important;
    margin: 0 !important;
    /* @page margins are unreliable in Chrome PDF export; pad content instead */
    padding: 18mm !important;
    box-sizing: border-box !important;
  }

  .content::before,
  .content::after {
    display: none !important;
  }

  .content [id] {
    scroll-margin-top: 0 !important;
  }

  .content h1 {
    margin-top: 0 !important;
    margin-left: 0 !important;
    padding-left: 0 !important;
  }

  .content ul li:before {
    content: '◦' !important;
  }

  .content ol li:before {
    content: counter(count)'.' !important;
  }

  table {
    break-inside: avoid;
    page-break-inside: avoid;
  }

  thead {
    display: table-header-group;
  }

  h1, h2, h3, h4, h5, h6 {
    break-after: avoid;
    page-break-after: avoid;
  }

  p, li, blockquote {
    orphans: 3;
    widows: 3;
  }

  /* Dark theme — always used for print/PDF */
  body {
    background: #0c1017 !important;
    color: #cbd5e1 !important;
  }

  .content h1,
  .content h2,
  .content h3,
  .content h4,
  .content h5 {
    color: #f1f5f9 !important;
  }

  .content h2 {
    padding-left: 0.75rem !important;
    border-left: 3px solid #14b8a6 !important;
  }

  .content hr {
    height: 1px !important;
    margin-top: 2rem !important;
    background: linear-gradient(90deg, #14b8a6, #334155, transparent) !important;
  }

  .content a:not(.header-link) {
    color: #2dd4bf !important;
    text-decoration: underline !important;
    text-decoration-color: rgba(45, 212, 191, 0.45) !important;
  }

  .content strong {
    color: #f1f5f9 !important;
  }

  .content code {
    background: #042f2e !important;
    color: #5eead4 !important;
  }

  .content pre code {
    background: #070a0f !important;
    color: #cbd5e1 !important;
    border: 1px solid #1e293b !important;
  }

  table {
    background: #0f1419 !important;
    color: #cbd5e1 !important;
  }

  th,
  td {
    border-color: #1e293b !important;
  }

  thead th {
    background: #111827 !important;
    color: #f1f5f9 !important;
    border-bottom-color: #14b8a6 !important;
  }

  tbody tr:nth-child(even) {
    background: rgba(255, 255, 255, 0.03) !important;
  }

  caption {
    color: #64748b !important;
  }
}
</style>
