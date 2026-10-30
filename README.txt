Chùa Liên Hoa (chualienhoa.org) - static HTML version
=====================================================

Upload the CONTENTS of this folder (including the hidden .htaccess file) to the web root of
chualienhoa.org, or to any subfolder for a staging preview. All links are relative.

Pages (same URLs as the live site)
  /                      -> index.html  (the summer retreat invitation)
  /sample-page/          -> WordPress sample page
  /author/AdminPhong/    -> author page

Not included
------------
- /form/en/ and /form/vi/: both already show WordPress's "The site is experiencing technical
  difficulties" error (500) on the live site, so there was nothing to copy.

Notes
-----
- The contact email on the home page was hidden by Cloudflare's email protection; it is now
  written out as plain text.
- The search box now opens a Google search limited to chualienhoa.org.

Noindex (staging)
-----------------
Every page has <meta name="robots" content="noindex, nofollow" /> and .htaccess sends an
X-Robots-Tag: noindex, nofollow header, so search engines will not index this copy.
BEFORE GOING LIVE on the real domain: remove that meta line from each page and delete the
"BEGIN noindex ... END noindex" block from .htaccess, or the site will drop out of Google.
