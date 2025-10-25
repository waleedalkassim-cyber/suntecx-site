Suntecx — Static Website Package (One Page)
===========================================

Files:
- index.html        (main site; references local ./logo.png)
- logo.png          (your logo; shown in header)
- index-inline.html (single-file demo with embedded base64 logo)

How to deploy on Vercel (static, no build step):
1) Go to https://vercel.com  → Add New → Project → Other.
2) Drag the UNZIPPED folder that contains index.html and logo.png.
3) Leave Build Command empty; Output directory as / (root).
4) Deploy. You’ll get a *.vercel.app URL.

Connect your domain (suntecx.ca):
- In Project → Settings → Domains add: suntecx.ca and www.suntecx.ca
- At your registrar DNS set:
  A     @     76.76.21.21
  CNAME www   cname.vercel-dns.com
- Remove conflicting/old A/AAAA/CNAME records.
- Wait a few minutes, then verify in Vercel.
