# Comparing `tmp/pollstats-0.5.tar.gz` & `tmp/pollstats-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pollstats-0.5.tar", last modified: Thu Apr 27 17:41:20 2023, max compression
+gzip compressed data, was "dist\pollstats-0.6.tar", last modified: Thu Apr 27 23:54:23 2023, max compression
```

## Comparing `pollstats-0.5.tar` & `pollstats-0.6.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/
--rw-rw-rw-   0        0        0     1055 2023-04-27 09:13:20.000000 pollstats-0.5/LICENSE
--rw-rw-rw-   0        0        0      113 2023-04-27 11:17:02.000000 pollstats-0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2887 2023-04-27 17:41:20.000000 pollstats-0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2168 2023-04-27 09:12:09.000000 pollstats-0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/
--rw-rw-rw-   0        0        0        0 2023-04-27 05:45:06.000000 pollstats-0.5/pollstats/__init__.py
--rw-rw-rw-   0        0        0       66 2023-04-27 05:45:06.000000 pollstats-0.5/pollstats/admin.py
--rw-rw-rw-   0        0        0      156 2023-04-27 05:45:06.000000 pollstats-0.5/pollstats/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/migrations/
--rw-rw-rw-   0        0        0        0 2023-04-27 05:45:06.000000 pollstats-0.5/pollstats/migrations/__init__.py
--rw-rw-rw-   0        0        0       60 2023-04-27 05:45:06.000000 pollstats-0.5/pollstats/models.py
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/static/
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/static/pollstatsassets/
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/static/pollstatsassets/css/
--rw-rw-rw-   0        0        0    41830 2023-04-24 10:04:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/css/style.css
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/
--rw-rw-rw-   0        0        0   193104 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/about.jpg
--rw-rw-rw-   0        0        0     1738 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/apple-touch-icon.png
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/blog/
--rw-rw-rw-   0        0        0    83878 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/blog/blog-1.jpg
--rw-rw-rw-   0        0        0   112816 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/blog/blog-2.jpg
--rw-rw-rw-   0        0        0    93369 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/blog/blog-3.jpg
--rw-rw-rw-   0        0        0   104099 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/blog/blog-4.jpg
--rw-rw-rw-   0        0        0    64790 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/blog/blog-author.jpg
--rw-rw-rw-   0        0        0    85335 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/blog/blog-inside-post.jpg
--rw-rw-rw-   0        0        0    83411 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/blog/blog-recent-1.jpg
--rw-rw-rw-   0        0        0    78239 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/blog/blog-recent-2.jpg
--rw-rw-rw-   0        0        0    71055 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/blog/blog-recent-3.jpg
--rw-rw-rw-   0        0        0   115012 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/blog/blog-recent-4.jpg
--rw-rw-rw-   0        0        0    93369 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/blog/blog-recent-5.jpg
--rw-rw-rw-   0        0        0    17444 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/blog/comments-1.jpg
--rw-rw-rw-   0        0        0    15407 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/blog/comments-2.jpg
--rw-rw-rw-   0        0        0    17041 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/blog/comments-3.jpg
--rw-rw-rw-   0        0        0    17774 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/blog/comments-4.jpg
--rw-rw-rw-   0        0        0    10855 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/blog/comments-5.jpg
--rw-rw-rw-   0        0        0    14253 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/blog/comments-6.jpg
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/clients/
--rw-rw-rw-   0        0        0     5282 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/clients/client-1.png
--rw-rw-rw-   0        0        0     4582 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/clients/client-2.png
--rw-rw-rw-   0        0        0     4707 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/clients/client-3.png
--rw-rw-rw-   0        0        0     9010 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/clients/client-4.png
--rw-rw-rw-   0        0        0     5123 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/clients/client-5.png
--rw-rw-rw-   0        0        0     3450 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/clients/client-6.png
--rw-rw-rw-   0        0        0     5616 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/clients/client-7.png
--rw-rw-rw-   0        0        0     4587 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/clients/client-8.png
--rw-rw-rw-   0        0        0      491 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/favicon.png
--rw-rw-rw-   0        0        0    44762 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/features-2.png
--rw-rw-rw-   0        0        0    33389 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/features-3.png
--rw-rw-rw-   0        0        0    55886 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/features.png
--rw-rw-rw-   0        0        0    10959 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/footer-bg.png
--rw-rw-rw-   0        0        0     7253 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/hero-bg.png
--rw-rw-rw-   0        0        0    22636 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/hero-img.png
--rw-rw-rw-   0        0        0    12137 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/hero-img.svg
--rw-rw-rw-   0        0        0     1071 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/logo.png
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/portfolio/
--rw-rw-rw-   0        0        0    82156 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/portfolio/portfolio-1.jpg
--rw-rw-rw-   0        0        0   100174 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/portfolio/portfolio-2.jpg
--rw-rw-rw-   0        0        0    12377 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/portfolio/portfolio-3.jpg
--rw-rw-rw-   0        0        0    72084 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/portfolio/portfolio-4.jpg
--rw-rw-rw-   0        0        0    81363 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/portfolio/portfolio-5.jpg
--rw-rw-rw-   0        0        0    25598 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/portfolio/portfolio-6.jpg
--rw-rw-rw-   0        0        0   122008 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/portfolio/portfolio-7.jpg
--rw-rw-rw-   0        0        0    15876 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/portfolio/portfolio-8.jpg
--rw-rw-rw-   0        0        0    58756 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/portfolio/portfolio-9.jpg
--rw-rw-rw-   0        0        0    10763 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/pricing-business.png
--rw-rw-rw-   0        0        0     6518 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/pricing-free.png
--rw-rw-rw-   0        0        0     8215 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/pricing-starter.png
--rw-rw-rw-   0        0        0     8139 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/pricing-ultimate.png
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/team/
--rw-rw-rw-   0        0        0    40201 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/team/team-1.jpg
--rw-rw-rw-   0        0        0    49059 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/team/team-2.jpg
--rw-rw-rw-   0        0        0    36680 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/team/team-3.jpg
--rw-rw-rw-   0        0        0    27423 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/team/team-4.jpg
--rw-rw-rw-   0        0        0      552 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/team-shape.svg
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/testimonials/
--rw-rw-rw-   0        0        0    39727 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/testimonials/testimonials-1.jpg
--rw-rw-rw-   0        0        0    57584 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/testimonials/testimonials-2.jpg
--rw-rw-rw-   0        0        0    17247 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/testimonials/testimonials-3.jpg
--rw-rw-rw-   0        0        0    20220 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/testimonials/testimonials-4.jpg
--rw-rw-rw-   0        0        0    22595 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/testimonials/testimonials-5.jpg
--rw-rw-rw-   0        0        0    20762 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/values-1.png
--rw-rw-rw-   0        0        0    22703 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/values-2.png
--rw-rw-rw-   0        0        0    20066 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/img/values-3.png
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/static/pollstatsassets/js/
--rw-rw-rw-   0        0        0     6883 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/js/main.js
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/static/pollstatsassets/scss/
--rw-rw-rw-   0        0        0       61 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/scss/Readme.txt
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/aos/
--rw-rw-rw-   0        0        0    26053 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/aos/aos.css
--rw-rw-rw-   0        0        0    14690 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/aos/aos.js
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/
--rw-rw-rw-   0        0        0    71861 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.css
--rw-rw-rw-   0        0        0   210357 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.css.map
--rw-rw-rw-   0        0        0    53265 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.min.css
--rw-rw-rw-   0        0        0   131395 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.min.css.map
--rw-rw-rw-   0        0        0    71935 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.rtl.css
--rw-rw-rw-   0        0        0   210361 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
--rw-rw-rw-   0        0        0    53340 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
--rw-rw-rw-   0        0        0   131472 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
--rw-rw-rw-   0        0        0     7965 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.css
--rw-rw-rw-   0        0        0   110875 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.css.map
--rw-rw-rw-   0        0        0     6490 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.min.css
--rw-rw-rw-   0        0        0    40331 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.min.css.map
--rw-rw-rw-   0        0        0     7958 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.rtl.css
--rw-rw-rw-   0        0        0   110888 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
--rw-rw-rw-   0        0        0     6562 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
--rw-rw-rw-   0        0        0    48693 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
--rw-rw-rw-   0        0        0    76347 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.css
--rw-rw-rw-   0        0        0   212450 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.css.map
--rw-rw-rw-   0        0        0    58266 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.min.css
--rw-rw-rw-   0        0        0   131956 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.min.css.map
--rw-rw-rw-   0        0        0    76214 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.rtl.css
--rw-rw-rw-   0        0        0   212393 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
--rw-rw-rw-   0        0        0    58194 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
--rw-rw-rw-   0        0        0   131791 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
--rw-rw-rw-   0        0        0   237950 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.css
--rw-rw-rw-   0        0        0   608300 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.css.map
--rw-rw-rw-   0        0        0   194901 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.min.css
--rw-rw-rw-   0        0        0   522639 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.min.css.map
--rw-rw-rw-   0        0        0   237528 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.rtl.css
--rw-rw-rw-   0        0        0   608144 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.rtl.css.map
--rw-rw-rw-   0        0        0   195007 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.rtl.min.css
--rw-rw-rw-   0        0        0   767483 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.rtl.min.css.map
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/js/
--rw-rw-rw-   0        0        0   207989 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.bundle.js
--rw-rw-rw-   0        0        0   451770 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.bundle.js.map
--rw-rw-rw-   0        0        0    80420 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0   333078 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.bundle.min.js.map
--rw-rw-rw-   0        0        0   136215 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.esm.js
--rw-rw-rw-   0        0        0   308207 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.esm.js.map
--rw-rw-rw-   0        0        0    73978 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.esm.min.js
--rw-rw-rw-   0        0        0   221179 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.esm.min.js.map
--rw-rw-rw-   0        0        0   145543 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.js
--rw-rw-rw-   0        0        0   309348 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.js.map
--rw-rw-rw-   0        0        0    60404 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.min.js
--rw-rw-rw-   0        0        0   216913 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.min.js.map
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap-icons/
--rw-rw-rw-   0        0        0    95609 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap-icons/bootstrap-icons.css
--rw-rw-rw-   0        0        0    51087 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap-icons/bootstrap-icons.json
--rw-rw-rw-   0        0        0   228090 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap-icons/bootstrap-icons.scss
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap-icons/fonts/
--rw-rw-rw-   0        0        0   164352 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
--rw-rw-rw-   0        0        0   121296 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/glightbox/
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/glightbox/css/
--rw-rw-rw-   0        0        0    17372 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/glightbox/css/glightbox.css
--rw-rw-rw-   0        0        0    13749 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/glightbox/css/glightbox.min.css
--rw-rw-rw-   0        0        0    52561 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/glightbox/css/plyr.css
--rw-rw-rw-   0        0        0    45081 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/glightbox/css/plyr.min.css
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/glightbox/js/
--rw-rw-rw-   0        0        0   109391 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/glightbox/js/glightbox.js
--rw-rw-rw-   0        0        0    55880 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/glightbox/js/glightbox.min.js
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/isotope-layout/
--rw-rw-rw-   0        0        0    91398 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/isotope-layout/isotope.pkgd.js
--rw-rw-rw-   0        0        0    35445 2023-04-24 08:52:51.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/isotope-layout/isotope.pkgd.min.js
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/php-email-form/
--rw-rw-rw-   0        0        0     2734 2023-04-24 08:52:52.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/php-email-form/validate.js
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/purecounter/
--rw-rw-rw-   0        0        0     5417 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/purecounter/purecounter_vanilla.js
--rw-rw-rw-   0        0        0    24750 2023-04-24 08:52:50.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/purecounter/purecounter_vanilla.js.map
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/remixicon/
--rw-rw-rw-   0        0        0   110438 2023-04-24 08:52:52.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.css
--rw-rw-rw-   0        0        0   403228 2023-04-24 08:52:52.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.eot
--rw-rw-rw-   0        0        0   110450 2023-04-24 08:52:52.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.less
--rw-rw-rw-   0        0        0  1195522 2023-04-24 08:52:52.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.svg
--rw-rw-rw-   0        0        0   897931 2023-04-24 08:52:52.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.symbol.svg
--rw-rw-rw-   0        0        0   403056 2023-04-24 08:52:52.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.ttf
--rw-rw-rw-   0        0        0   172876 2023-04-24 08:52:52.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.woff
--rw-rw-rw-   0        0        0   125268 2023-04-24 08:52:52.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.woff2
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/swiper/
--rw-rw-rw-   0        0        0    16493 2023-04-24 08:52:52.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/swiper/swiper-bundle.min.css
--rw-rw-rw-   0        0        0   143706 2023-04-24 08:52:52.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/swiper/swiper-bundle.min.js
--rw-rw-rw-   0        0        0   540665 2023-04-24 08:52:52.000000 pollstats-0.5/pollstats/static/pollstatsassets/vendor/swiper/swiper-bundle.min.js.map
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats/templates/
--rw-rw-rw-   0        0        0     3283 2023-04-27 06:53:44.000000 pollstats-0.5/pollstats/templates/stats.html
--rw-rw-rw-   0        0        0       63 2023-04-27 05:45:06.000000 pollstats-0.5/pollstats/tests.py
--rw-rw-rw-   0        0        0      135 2023-04-27 06:34:19.000000 pollstats-0.5/pollstats/urls.py
--rw-rw-rw-   0        0        0      909 2023-04-27 17:39:58.000000 pollstats-0.5/pollstats/views.py
-drwxrwxrwx   0        0        0        0 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats.egg-info/
--rw-rw-rw-   0        0        0     2887 2023-04-27 17:41:19.000000 pollstats-0.5/pollstats.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9503 2023-04-27 17:41:20.000000 pollstats-0.5/pollstats.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 17:41:19.000000 pollstats-0.5/pollstats.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-27 17:41:19.000000 pollstats-0.5/pollstats.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      546 2023-04-27 09:52:29.000000 pollstats-0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 17:41:20.000000 pollstats-0.5/setup.cfg
--rw-rw-rw-   0        0        0      946 2023-04-27 17:40:41.000000 pollstats-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:23.000000 pollstats-0.6/
+-rw-rw-rw-   0        0        0     1055 2023-04-27 09:13:20.000000 pollstats-0.6/LICENSE
+-rw-rw-rw-   0        0        0      113 2023-04-27 11:17:02.000000 pollstats-0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2887 2023-04-27 23:54:23.000000 pollstats-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2168 2023-04-27 09:12:09.000000 pollstats-0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:21.000000 pollstats-0.6/pollstats/
+-rw-rw-rw-   0        0        0        0 2023-04-27 05:45:06.000000 pollstats-0.6/pollstats/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-04-27 05:45:06.000000 pollstats-0.6/pollstats/admin.py
+-rw-rw-rw-   0        0        0      156 2023-04-27 05:45:06.000000 pollstats-0.6/pollstats/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:21.000000 pollstats-0.6/pollstats/migrations/
+-rw-rw-rw-   0        0        0        0 2023-04-27 05:45:06.000000 pollstats-0.6/pollstats/migrations/__init__.py
+-rw-rw-rw-   0        0        0       60 2023-04-27 05:45:06.000000 pollstats-0.6/pollstats/models.py
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:21.000000 pollstats-0.6/pollstats/static/
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:21.000000 pollstats-0.6/pollstats/static/pollstatsassets/
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:21.000000 pollstats-0.6/pollstats/static/pollstatsassets/css/
+-rw-rw-rw-   0        0        0    41830 2023-04-24 10:04:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/css/style.css
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:21.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/
+-rw-rw-rw-   0        0        0   193104 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/about.jpg
+-rw-rw-rw-   0        0        0     1738 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/apple-touch-icon.png
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:21.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/blog/
+-rw-rw-rw-   0        0        0    83878 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/blog/blog-1.jpg
+-rw-rw-rw-   0        0        0   112816 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/blog/blog-2.jpg
+-rw-rw-rw-   0        0        0    93369 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/blog/blog-3.jpg
+-rw-rw-rw-   0        0        0   104099 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/blog/blog-4.jpg
+-rw-rw-rw-   0        0        0    64790 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/blog/blog-author.jpg
+-rw-rw-rw-   0        0        0    85335 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/blog/blog-inside-post.jpg
+-rw-rw-rw-   0        0        0    83411 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/blog/blog-recent-1.jpg
+-rw-rw-rw-   0        0        0    78239 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/blog/blog-recent-2.jpg
+-rw-rw-rw-   0        0        0    71055 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/blog/blog-recent-3.jpg
+-rw-rw-rw-   0        0        0   115012 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/blog/blog-recent-4.jpg
+-rw-rw-rw-   0        0        0    93369 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/blog/blog-recent-5.jpg
+-rw-rw-rw-   0        0        0    17444 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/blog/comments-1.jpg
+-rw-rw-rw-   0        0        0    15407 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/blog/comments-2.jpg
+-rw-rw-rw-   0        0        0    17041 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/blog/comments-3.jpg
+-rw-rw-rw-   0        0        0    17774 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/blog/comments-4.jpg
+-rw-rw-rw-   0        0        0    10855 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/blog/comments-5.jpg
+-rw-rw-rw-   0        0        0    14253 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/blog/comments-6.jpg
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:21.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/clients/
+-rw-rw-rw-   0        0        0     5282 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/clients/client-1.png
+-rw-rw-rw-   0        0        0     4582 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/clients/client-2.png
+-rw-rw-rw-   0        0        0     4707 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/clients/client-3.png
+-rw-rw-rw-   0        0        0     9010 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/clients/client-4.png
+-rw-rw-rw-   0        0        0     5123 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/clients/client-5.png
+-rw-rw-rw-   0        0        0     3450 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/clients/client-6.png
+-rw-rw-rw-   0        0        0     5616 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/clients/client-7.png
+-rw-rw-rw-   0        0        0     4587 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/clients/client-8.png
+-rw-rw-rw-   0        0        0      491 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/favicon.png
+-rw-rw-rw-   0        0        0    44762 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/features-2.png
+-rw-rw-rw-   0        0        0    33389 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/features-3.png
+-rw-rw-rw-   0        0        0    55886 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/features.png
+-rw-rw-rw-   0        0        0    10959 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/footer-bg.png
+-rw-rw-rw-   0        0        0     7253 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/hero-bg.png
+-rw-rw-rw-   0        0        0    22636 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/hero-img.png
+-rw-rw-rw-   0        0        0    12137 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/hero-img.svg
+-rw-rw-rw-   0        0        0     1071 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/logo.png
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:21.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/portfolio/
+-rw-rw-rw-   0        0        0    82156 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/portfolio/portfolio-1.jpg
+-rw-rw-rw-   0        0        0   100174 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/portfolio/portfolio-2.jpg
+-rw-rw-rw-   0        0        0    12377 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/portfolio/portfolio-3.jpg
+-rw-rw-rw-   0        0        0    72084 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/portfolio/portfolio-4.jpg
+-rw-rw-rw-   0        0        0    81363 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/portfolio/portfolio-5.jpg
+-rw-rw-rw-   0        0        0    25598 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/portfolio/portfolio-6.jpg
+-rw-rw-rw-   0        0        0   122008 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/portfolio/portfolio-7.jpg
+-rw-rw-rw-   0        0        0    15876 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/portfolio/portfolio-8.jpg
+-rw-rw-rw-   0        0        0    58756 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/portfolio/portfolio-9.jpg
+-rw-rw-rw-   0        0        0    10763 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/pricing-business.png
+-rw-rw-rw-   0        0        0     6518 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/pricing-free.png
+-rw-rw-rw-   0        0        0     8215 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/pricing-starter.png
+-rw-rw-rw-   0        0        0     8139 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/pricing-ultimate.png
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:21.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/team/
+-rw-rw-rw-   0        0        0    40201 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/team/team-1.jpg
+-rw-rw-rw-   0        0        0    49059 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/team/team-2.jpg
+-rw-rw-rw-   0        0        0    36680 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/team/team-3.jpg
+-rw-rw-rw-   0        0        0    27423 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/team/team-4.jpg
+-rw-rw-rw-   0        0        0      552 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/team-shape.svg
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:21.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/testimonials/
+-rw-rw-rw-   0        0        0    39727 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/testimonials/testimonials-1.jpg
+-rw-rw-rw-   0        0        0    57584 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/testimonials/testimonials-2.jpg
+-rw-rw-rw-   0        0        0    17247 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/testimonials/testimonials-3.jpg
+-rw-rw-rw-   0        0        0    20220 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/testimonials/testimonials-4.jpg
+-rw-rw-rw-   0        0        0    22595 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/testimonials/testimonials-5.jpg
+-rw-rw-rw-   0        0        0    20762 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/values-1.png
+-rw-rw-rw-   0        0        0    22703 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/values-2.png
+-rw-rw-rw-   0        0        0    20066 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/img/values-3.png
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:21.000000 pollstats-0.6/pollstats/static/pollstatsassets/js/
+-rw-rw-rw-   0        0        0     6883 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/js/main.js
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:21.000000 pollstats-0.6/pollstats/static/pollstatsassets/scss/
+-rw-rw-rw-   0        0        0       61 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/scss/Readme.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:21.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:21.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/aos/
+-rw-rw-rw-   0        0        0    26053 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/aos/aos.css
+-rw-rw-rw-   0        0        0    14690 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/aos/aos.js
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:21.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:22.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/
+-rw-rw-rw-   0        0        0    71861 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.css
+-rw-rw-rw-   0        0        0   210357 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.css.map
+-rw-rw-rw-   0        0        0    53265 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.min.css
+-rw-rw-rw-   0        0        0   131395 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.min.css.map
+-rw-rw-rw-   0        0        0    71935 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.rtl.css
+-rw-rw-rw-   0        0        0   210361 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
+-rw-rw-rw-   0        0        0    53340 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
+-rw-rw-rw-   0        0        0   131472 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
+-rw-rw-rw-   0        0        0     7965 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.css
+-rw-rw-rw-   0        0        0   110875 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.css.map
+-rw-rw-rw-   0        0        0     6490 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.min.css
+-rw-rw-rw-   0        0        0    40331 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-rw-rw-   0        0        0     7958 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.rtl.css
+-rw-rw-rw-   0        0        0   110888 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
+-rw-rw-rw-   0        0        0     6562 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
+-rw-rw-rw-   0        0        0    48693 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
+-rw-rw-rw-   0        0        0    76347 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.css
+-rw-rw-rw-   0        0        0   212450 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.css.map
+-rw-rw-rw-   0        0        0    58266 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.min.css
+-rw-rw-rw-   0        0        0   131956 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.min.css.map
+-rw-rw-rw-   0        0        0    76214 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.rtl.css
+-rw-rw-rw-   0        0        0   212393 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
+-rw-rw-rw-   0        0        0    58194 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
+-rw-rw-rw-   0        0        0   131791 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
+-rw-rw-rw-   0        0        0   237950 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.css
+-rw-rw-rw-   0        0        0   608300 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.css.map
+-rw-rw-rw-   0        0        0   194901 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0   522639 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.min.css.map
+-rw-rw-rw-   0        0        0   237528 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.rtl.css
+-rw-rw-rw-   0        0        0   608144 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.rtl.css.map
+-rw-rw-rw-   0        0        0   195007 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.rtl.min.css
+-rw-rw-rw-   0        0        0   767483 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.rtl.min.css.map
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:22.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/js/
+-rw-rw-rw-   0        0        0   207989 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.bundle.js
+-rw-rw-rw-   0        0        0   451770 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.bundle.js.map
+-rw-rw-rw-   0        0        0    80420 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0   333078 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-rw-rw-   0        0        0   136215 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.esm.js
+-rw-rw-rw-   0        0        0   308207 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.esm.js.map
+-rw-rw-rw-   0        0        0    73978 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.esm.min.js
+-rw-rw-rw-   0        0        0   221179 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.esm.min.js.map
+-rw-rw-rw-   0        0        0   145543 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.js
+-rw-rw-rw-   0        0        0   309348 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.js.map
+-rw-rw-rw-   0        0        0    60404 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0   216913 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.min.js.map
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:21.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap-icons/
+-rw-rw-rw-   0        0        0    95609 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap-icons/bootstrap-icons.css
+-rw-rw-rw-   0        0        0    51087 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap-icons/bootstrap-icons.json
+-rw-rw-rw-   0        0        0   228090 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap-icons/bootstrap-icons.scss
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:21.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap-icons/fonts/
+-rw-rw-rw-   0        0        0   164352 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
+-rw-rw-rw-   0        0        0   121296 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:21.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/glightbox/
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:22.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/glightbox/css/
+-rw-rw-rw-   0        0        0    17372 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/glightbox/css/glightbox.css
+-rw-rw-rw-   0        0        0    13749 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/glightbox/css/glightbox.min.css
+-rw-rw-rw-   0        0        0    52561 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/glightbox/css/plyr.css
+-rw-rw-rw-   0        0        0    45081 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/glightbox/css/plyr.min.css
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:22.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/glightbox/js/
+-rw-rw-rw-   0        0        0   109391 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/glightbox/js/glightbox.js
+-rw-rw-rw-   0        0        0    55880 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/glightbox/js/glightbox.min.js
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:22.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/isotope-layout/
+-rw-rw-rw-   0        0        0    91398 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/isotope-layout/isotope.pkgd.js
+-rw-rw-rw-   0        0        0    35445 2023-04-24 08:52:51.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/isotope-layout/isotope.pkgd.min.js
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:22.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/php-email-form/
+-rw-rw-rw-   0        0        0     2734 2023-04-24 08:52:52.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/php-email-form/validate.js
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:22.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/purecounter/
+-rw-rw-rw-   0        0        0     5417 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/purecounter/purecounter_vanilla.js
+-rw-rw-rw-   0        0        0    24750 2023-04-24 08:52:50.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/purecounter/purecounter_vanilla.js.map
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:22.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/remixicon/
+-rw-rw-rw-   0        0        0   110438 2023-04-24 08:52:52.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.css
+-rw-rw-rw-   0        0        0   403228 2023-04-24 08:52:52.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.eot
+-rw-rw-rw-   0        0        0   110450 2023-04-24 08:52:52.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.less
+-rw-rw-rw-   0        0        0  1195522 2023-04-24 08:52:52.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.svg
+-rw-rw-rw-   0        0        0   897931 2023-04-24 08:52:52.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.symbol.svg
+-rw-rw-rw-   0        0        0   403056 2023-04-24 08:52:52.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.ttf
+-rw-rw-rw-   0        0        0   172876 2023-04-24 08:52:52.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.woff
+-rw-rw-rw-   0        0        0   125268 2023-04-24 08:52:52.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.woff2
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:23.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/swiper/
+-rw-rw-rw-   0        0        0    16493 2023-04-24 08:52:52.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/swiper/swiper-bundle.min.css
+-rw-rw-rw-   0        0        0   143706 2023-04-24 08:52:52.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/swiper/swiper-bundle.min.js
+-rw-rw-rw-   0        0        0   540665 2023-04-24 08:52:52.000000 pollstats-0.6/pollstats/static/pollstatsassets/vendor/swiper/swiper-bundle.min.js.map
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:23.000000 pollstats-0.6/pollstats/templates/
+-rw-rw-rw-   0        0        0     3283 2023-04-27 06:53:44.000000 pollstats-0.6/pollstats/templates/stats.html
+-rw-rw-rw-   0        0        0       63 2023-04-27 05:45:06.000000 pollstats-0.6/pollstats/tests.py
+-rw-rw-rw-   0        0        0      135 2023-04-27 06:34:19.000000 pollstats-0.6/pollstats/urls.py
+-rw-rw-rw-   0        0        0      921 2023-04-27 23:50:19.000000 pollstats-0.6/pollstats/views.py
+drwxrwxrwx   0        0        0        0 2023-04-27 23:54:21.000000 pollstats-0.6/pollstats.egg-info/
+-rw-rw-rw-   0        0        0     2887 2023-04-27 23:54:21.000000 pollstats-0.6/pollstats.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9503 2023-04-27 23:54:21.000000 pollstats-0.6/pollstats.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 23:54:21.000000 pollstats-0.6/pollstats.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-27 23:54:21.000000 pollstats-0.6/pollstats.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      546 2023-04-27 09:52:29.000000 pollstats-0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 23:54:23.000000 pollstats-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      946 2023-04-27 23:51:44.000000 pollstats-0.6/setup.py
```

### Comparing `pollstats-0.5/LICENSE` & `pollstats-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/PKG-INFO` & `pollstats-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollstats
-Version: 0.5
+Version: 0.6
 Summary: A short description of your package
 Home-page: https://github.com/Vijayanand-debug/pollstats
 Author: Vijayanand
 Author-email: vijayanand563@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pollstats-0.5/README.md` & `pollstats-0.6/README.md`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/css/style.css` & `pollstats-0.6/pollstats/static/pollstatsassets/css/style.css`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/about.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/about.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/apple-touch-icon.png` & `pollstats-0.6/pollstats/static/pollstatsassets/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/blog/blog-1.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/blog/blog-1.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/blog/blog-2.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/blog/blog-2.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/blog/blog-3.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/blog/blog-3.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/blog/blog-4.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/blog/blog-4.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/blog/blog-author.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/blog/blog-author.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/blog/blog-inside-post.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/blog/blog-inside-post.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/blog/blog-recent-1.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/blog/blog-recent-1.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/blog/blog-recent-2.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/blog/blog-recent-2.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/blog/blog-recent-3.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/blog/blog-recent-3.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/blog/blog-recent-4.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/blog/blog-recent-4.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/blog/blog-recent-5.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/blog/blog-recent-5.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/blog/comments-1.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/blog/comments-1.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/blog/comments-2.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/blog/comments-2.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/blog/comments-3.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/blog/comments-3.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/blog/comments-4.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/blog/comments-4.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/blog/comments-5.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/blog/comments-5.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/blog/comments-6.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/blog/comments-6.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/clients/client-1.png` & `pollstats-0.6/pollstats/static/pollstatsassets/img/clients/client-1.png`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/clients/client-2.png` & `pollstats-0.6/pollstats/static/pollstatsassets/img/clients/client-2.png`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/clients/client-3.png` & `pollstats-0.6/pollstats/static/pollstatsassets/img/clients/client-3.png`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/clients/client-4.png` & `pollstats-0.6/pollstats/static/pollstatsassets/img/clients/client-4.png`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/clients/client-5.png` & `pollstats-0.6/pollstats/static/pollstatsassets/img/clients/client-5.png`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/clients/client-6.png` & `pollstats-0.6/pollstats/static/pollstatsassets/img/clients/client-6.png`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/clients/client-7.png` & `pollstats-0.6/pollstats/static/pollstatsassets/img/clients/client-7.png`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/clients/client-8.png` & `pollstats-0.6/pollstats/static/pollstatsassets/img/clients/client-8.png`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/features-2.png` & `pollstats-0.6/pollstats/static/pollstatsassets/img/features-2.png`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/features-3.png` & `pollstats-0.6/pollstats/static/pollstatsassets/img/features-3.png`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/features.png` & `pollstats-0.6/pollstats/static/pollstatsassets/img/features.png`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/footer-bg.png` & `pollstats-0.6/pollstats/static/pollstatsassets/img/footer-bg.png`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/hero-bg.png` & `pollstats-0.6/pollstats/static/pollstatsassets/img/hero-bg.png`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/hero-img.png` & `pollstats-0.6/pollstats/static/pollstatsassets/img/hero-img.png`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/hero-img.svg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/hero-img.svg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/logo.png` & `pollstats-0.6/pollstats/static/pollstatsassets/img/logo.png`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/portfolio/portfolio-1.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/portfolio/portfolio-1.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/portfolio/portfolio-2.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/portfolio/portfolio-2.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/portfolio/portfolio-3.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/portfolio/portfolio-3.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/portfolio/portfolio-4.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/portfolio/portfolio-4.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/portfolio/portfolio-5.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/portfolio/portfolio-5.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/portfolio/portfolio-6.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/portfolio/portfolio-6.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/portfolio/portfolio-7.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/portfolio/portfolio-7.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/portfolio/portfolio-8.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/portfolio/portfolio-8.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/portfolio/portfolio-9.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/portfolio/portfolio-9.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/pricing-business.png` & `pollstats-0.6/pollstats/static/pollstatsassets/img/pricing-business.png`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/pricing-free.png` & `pollstats-0.6/pollstats/static/pollstatsassets/img/pricing-free.png`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/pricing-starter.png` & `pollstats-0.6/pollstats/static/pollstatsassets/img/pricing-starter.png`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/pricing-ultimate.png` & `pollstats-0.6/pollstats/static/pollstatsassets/img/pricing-ultimate.png`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/team/team-1.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/team/team-1.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/team/team-2.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/team/team-2.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/team/team-3.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/team/team-3.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/team/team-4.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/team/team-4.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/team-shape.svg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/team-shape.svg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/testimonials/testimonials-1.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/testimonials/testimonials-1.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/testimonials/testimonials-2.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/testimonials/testimonials-2.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/testimonials/testimonials-3.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/testimonials/testimonials-3.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/testimonials/testimonials-4.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/testimonials/testimonials-4.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/testimonials/testimonials-5.jpg` & `pollstats-0.6/pollstats/static/pollstatsassets/img/testimonials/testimonials-5.jpg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/values-1.png` & `pollstats-0.6/pollstats/static/pollstatsassets/img/values-1.png`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/values-2.png` & `pollstats-0.6/pollstats/static/pollstatsassets/img/values-2.png`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/img/values-3.png` & `pollstats-0.6/pollstats/static/pollstatsassets/img/values-3.png`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/js/main.js` & `pollstats-0.6/pollstats/static/pollstatsassets/js/main.js`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/aos/aos.css` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/aos/aos.css`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/aos/aos.js` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/aos/aos.js`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.css` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.css.map` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.min.css` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.min.css.map` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.rtl.css` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.rtl.css.map` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.rtl.min.css` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.css` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.css.map` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.min.css` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.min.css.map` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.rtl.css` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.css` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.css.map` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.min.css` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.min.css.map` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.rtl.css` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.css` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.css.map` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.min.css` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.min.css.map` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.rtl.css` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.rtl.css.map` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.rtl.min.css` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.rtl.min.css.map` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.bundle.js` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.bundle.js.map` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.bundle.min.js` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.bundle.min.js.map` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.esm.js` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.esm.js.map` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.esm.min.js` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.esm.min.js.map` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.js` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.js.map` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.min.js` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.min.js.map` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap-icons/bootstrap-icons.css` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap-icons/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap-icons/bootstrap-icons.json` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap-icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap-icons/bootstrap-icons.scss` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap-icons/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap-icons/fonts/bootstrap-icons.woff` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap-icons/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/glightbox/css/glightbox.css` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/glightbox/css/glightbox.css`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/glightbox/css/glightbox.min.css` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/glightbox/css/glightbox.min.css`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/glightbox/css/plyr.css` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/glightbox/css/plyr.css`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/glightbox/css/plyr.min.css` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/glightbox/css/plyr.min.css`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/glightbox/js/glightbox.js` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/glightbox/js/glightbox.js`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/glightbox/js/glightbox.min.js` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/glightbox/js/glightbox.min.js`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/isotope-layout/isotope.pkgd.js` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/isotope-layout/isotope.pkgd.js`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/isotope-layout/isotope.pkgd.min.js` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/isotope-layout/isotope.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/php-email-form/validate.js` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/php-email-form/validate.js`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/purecounter/purecounter_vanilla.js` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/purecounter/purecounter_vanilla.js`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/purecounter/purecounter_vanilla.js.map` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/purecounter/purecounter_vanilla.js.map`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.css` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.css`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.eot` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.eot`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.less` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.less`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.svg` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.svg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.symbol.svg` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.symbol.svg`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.ttf` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.ttf`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.woff` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.woff`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.woff2` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/remixicon/remixicon.woff2`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/swiper/swiper-bundle.min.css` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/swiper/swiper-bundle.min.css`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/swiper/swiper-bundle.min.js` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/swiper/swiper-bundle.min.js`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/static/pollstatsassets/vendor/swiper/swiper-bundle.min.js.map` & `pollstats-0.6/pollstats/static/pollstatsassets/vendor/swiper/swiper-bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/templates/stats.html` & `pollstats-0.6/pollstats/templates/stats.html`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pollstats/views.py` & `pollstats-0.6/pollstats/views.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,14 @@
 
     transactions= Transactions.objects.filter(event_code=event_code)
     if transactions.exists:
      for t in transactions:
         transaction_count=transaction_count + 1
 
     if count > 0:
-      vote_percentage= (transaction_count/count) * 100
+      vote_percentage= round((transaction_count / count) * 100, 2)
       stats['entire_user_count'] = count
       stats['voted_count'] = transaction_count
       stats['vote_percent'] = vote_percentage
       stats['event_id'] = event_id
 
     return stats
```

### Comparing `pollstats-0.5/pollstats.egg-info/PKG-INFO` & `pollstats-0.6/pollstats.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollstats
-Version: 0.5
+Version: 0.6
 Summary: A short description of your package
 Home-page: https://github.com/Vijayanand-debug/pollstats
 Author: Vijayanand
 Author-email: vijayanand563@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pollstats-0.5/pollstats.egg-info/SOURCES.txt` & `pollstats-0.6/pollstats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/pyproject.toml` & `pollstats-0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pollstats-0.5/setup.py` & `pollstats-0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pollstats",
-    version="0.5",
+    version="0.6",
     packages=find_packages(),
     install_requires=[
         # List your package's dependencies here
 
     ],
     author="Vijayanand",
     author_email="vijayanand563@gmail.com",
```

