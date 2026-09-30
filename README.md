/* Abdul Kadir portfolio: styles.css
   Load fonts in your HTML <head>:
   <link href="https://fonts.googleapis.com/css2?family=Archivo:wdth,wght@75..100,500..800&family=Source+Sans+3:wght@400;600&display=swap" rel="stylesheet">
   Then: <link rel="stylesheet" href="styles.css"> */

:root{--bg:#F3F5F2;--card:#fff;--ink:#13232B;--muted:#52646C;--line:#C5CFCB;--accent:#0F5C5A;--hi:#F2B705;
--head:"Archivo","Arial Narrow",Arial,sans-serif;--body:"Source Sans 3",Segoe UI,Arial,sans-serif;
box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media (prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#0E1A1F;--card:#14252B;--ink:#E8EEEC;--muted:#93A5A8;--line:#2A3D43;--accent:#5CC7BF}}
:root[data-theme="dark"]{--bg:#0E1A1F;--card:#14252B;--ink:#E8EEEC;--muted:#93A5A8;--line:#2A3D43;--accent:#5CC7BF}
html{scroll-padding-top:calc(64px + env(safe-area-inset-top,0px));scroll-behavior:smooth}
*,*::before,*::after{box-sizing:border-box}
body{margin:0;background:var(--bg);color:var(--ink);font:18px/1.6 var(--body)}
a{color:var(--accent)}
:focus-visible{outline:3px solid var(--hi);outline-offset:2px}
.wrap{max-width:1040px;margin:0 auto;padding:0 20px}
nav{position:sticky;top:env(safe-area-inset-top,0px);z-index:5;background:var(--bg);border-bottom:1px solid var(--line)}
nav .wrap{display:flex;align-items:center;gap:20px;height:56px;overflow-x:auto;white-space:nowrap}
nav b{font:700 17px var(--head);margin-right:auto}
nav a{color:var(--muted);text-decoration:none;font-size:16px}
nav a:hover{color:var(--ink)}
nav button{background:none;border:1px solid var(--line);color:var(--ink);border-radius:6px;padding:4px 10px;font:inherit;font-size:15px;cursor:pointer}
h1,h2,h3{font-family:var(--head);line-height:1.1;margin:0}
section{padding:64px 0 8px}
h2{font-size:clamp(28px,4vw,38px);font-weight:700;font-stretch:80%;margin-bottom:24px}
.tb{margin:40px 0 0;border:2px solid var(--ink);background:var(--card);display:grid;grid-template-columns:repeat(6,1fr)}
.tb>div{padding:12px 16px;border-right:1px solid var(--ink);border-bottom:1px solid var(--ink)}
.tb small{display:block;color:var(--muted);font-size:14px}
.tb .name{grid-column:1/-1;border-right:0;padding:24px 16px 20px;background:var(--hi);color:#13232B}
.tb .name small{color:#3a3a20}
.tb h1{font-size:clamp(40px,9vw,88px);font-weight:800;font-stretch:76%;letter-spacing:-.01em}
.tb .c2{grid-column:span 2}.tb .c3{grid-column:span 3}
.tb>div:nth-child(n+2):nth-last-child(-n+3){border-bottom:0}
.lead{font-size:clamp(20px,2.4vw,24px);max-width:34em;margin:32px 0 20px}
.btns{display:flex;gap:12px;flex-wrap:wrap}
.btn{display:inline-block;padding:12px 20px;border:2px solid var(--ink);border-radius:4px;text-decoration:none;color:var(--ink);font-weight:600}
.btn.p{background:var(--ink);color:var(--bg)}
.two{display:grid;grid-template-columns:1fr 1fr;gap:32px}
p{margin:0 0 14px;max-width:40em}
.grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(230px,1fr));gap:0;border:1px solid var(--line);background:var(--card)}
.grid>div{padding:20px;border-right:1px solid var(--line);border-bottom:1px solid var(--line);margin:0 -1px -1px 0}
.grid h3{font-size:19px;margin-bottom:8px;font-weight:700}
.grid ul,.list{margin:0;padding-left:18px;color:var(--muted);font-size:16px}
.role{border-left:4px solid var(--accent);padding-left:20px;margin-bottom:28px}
.role h3{font-size:22px}.role .m{color:var(--muted);font-size:16px}
.scroll{overflow-x:auto;border:1px solid var(--line);background:var(--card)}
table{border-collapse:collapse;width:100%;min-width:640px;font-size:16px}
th,td{text-align:left;padding:12px 14px;border-bottom:1px solid var(--line);vertical-align:top}
th{font:600 15px var(--head);color:var(--muted)}
td.n{text-align:right;font-variant-numeric:tabular-nums;white-space:nowrap}
th.n{text-align:right}
tfoot td{font-weight:600;border-bottom:0;background:var(--bg)}
.note{color:var(--muted);font-size:15px;margin-top:10px}
.ed{display:grid;gap:14px}
.ed div{padding-bottom:14px;border-bottom:1px solid var(--line)}
.ed b{font-family:var(--head)}
footer{margin-top:72px;border-top:1px solid var(--line);padding:24px 0 40px;color:var(--muted);font-size:15px}
@media (max-width:720px){.tb{grid-template-columns:repeat(2,1fr)}.tb .c2,.tb .c3{grid-column:span 2}.tb>div{border-right:0}.two{grid-template-columns:1fr}}
@media (prefers-reduced-motion:reduce){html{scroll-behavior:auto}}
