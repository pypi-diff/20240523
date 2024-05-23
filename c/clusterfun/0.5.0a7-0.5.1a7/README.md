# Comparing `tmp/clusterfun-0.5.0a7.tar.gz` & `tmp/clusterfun-0.5.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clusterfun-0.5.0a7.tar", max compression
+gzip compressed data, was "clusterfun-0.5.1a7.tar", max compression
```

## Comparing `clusterfun-0.5.0a7.tar` & `clusterfun-0.5.1a7.tar`

### file list

```diff
@@ -1,130 +1,130 @@
--rw-r--r--   0        0        0    11357 2024-04-28 22:32:09.819834 clusterfun-0.5.0a7/LICENSE
--rw-r--r--   0        0        0     9280 2024-04-28 22:32:09.820288 clusterfun-0.5.0a7/README.md
--rw-r--r--   0        0        0      660 2024-04-28 22:32:09.852017 clusterfun-0.5.0a7/clusterfun/__init__.py
--rw-r--r--   0        0        0      970 2024-05-19 14:26:30.502142 clusterfun-0.5.0a7/clusterfun/app.py
--rw-r--r--   0        0        0     2750 2024-05-22 22:53:46.023349 clusterfun-0.5.0a7/clusterfun/config.py
--rw-r--r--   0        0        0      715 2024-04-28 22:32:09.852760 clusterfun-0.5.0a7/clusterfun/constants.py
--rw-r--r--   0        0        0     6790 2024-05-22 22:55:21.594564 clusterfun-0.5.0a7/clusterfun/frontend/404.html
--rw-r--r--   0        0        0      224 2024-05-02 18:20:15.920034 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/0L8U1RGbBQqzpAEgBP-4y/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-02 18:20:15.920441 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/0L8U1RGbBQqzpAEgBP-4y/_ssgManifest.js
--rw-r--r--   0        0        0      224 2024-05-07 09:53:06.289880 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/0t2IpDcBx6FIaFpL5-DTX/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-07 09:53:06.288728 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/0t2IpDcBx6FIaFpL5-DTX/_ssgManifest.js
--rw-r--r--   0        0        0      224 2024-05-01 14:48:56.190992 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/7K0stYTjLuE1ieiHwaOY8/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-01 14:48:56.191316 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/7K0stYTjLuE1ieiHwaOY8/_ssgManifest.js
--rw-r--r--   0        0        0      224 2024-05-01 14:48:56.192076 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/9m8W0thtsOjMrVxSpss7G/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-01 14:48:56.192715 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/9m8W0thtsOjMrVxSpss7G/_ssgManifest.js
--rw-r--r--   0        0        0      224 2024-05-02 18:20:15.921043 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/FajzyA8s2dBSB6nVAodLv/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-02 18:20:15.921298 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/FajzyA8s2dBSB6nVAodLv/_ssgManifest.js
--rw-r--r--   0        0        0      224 2024-05-22 22:55:21.599225 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/P5xyy85ON_Ic7d-vfYKXs/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-22 22:55:21.598755 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/P5xyy85ON_Ic7d-vfYKXs/_ssgManifest.js
--rw-r--r--   0        0        0      224 2024-05-19 14:37:19.186304 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/U2JWEnXogvGKNw9dZYznH/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-19 14:37:19.184257 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/U2JWEnXogvGKNw9dZYznH/_ssgManifest.js
--rw-r--r--   0        0        0     8025 2024-05-01 14:48:56.193828 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/22.94ebc66962dcd0f8.js
--rw-r--r--   0        0        0   121966 2024-05-19 14:37:19.168355 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/23-8126128752749016.js
--rw-r--r--   0        0        0   121966 2024-05-22 22:55:21.621856 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/23-916fe2f1983668e3.js
--rw-r--r--   0        0        0   110785 2024-05-01 14:48:56.198064 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/472-07a7dd51a787971b.js
--rw-r--r--   0        0        0   143320 2024-05-01 14:48:56.199462 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/483-2d99a375fdcaeaa9.js
--rw-r--r--   0        0        0   131700 2024-05-02 18:20:15.926209 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/500-9855c0cda36bb0be.js
--rw-r--r--   0        0        0   131700 2024-05-07 09:53:06.297351 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/500-9beb637c2f8db305.js
--rw-r--r--   0        0        0   146876 2024-05-22 22:55:21.627851 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/771-1510a54548bf26b3.js
--rw-r--r--   0        0        0     7388 2024-05-22 22:55:21.605280 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/8.d9282dffb5cd6834.js
--rw-r--r--   0        0        0   134273 2024-05-19 14:37:19.171903 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/86-fdf3fe7d49e1a681.js
--rw-r--r--   0        0        0     7683 2024-05-22 22:55:21.621352 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/870fdd6f-080da6c9b87ec5a2.js
--rw-r--r--   0        0        0     4290 2024-05-18 14:34:34.764454 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/870fdd6f-4049d31c55f7218c.js
--rw-r--r--   0        0        0     4290 2024-05-01 14:48:56.203293 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/870fdd6f-51765f2c6413dd54.js
--rw-r--r--   0        0        0     5079 2024-05-19 14:37:19.173787 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/870fdd6f-728b0ab9f208053f.js
--rw-r--r--   0        0        0     1744 2024-05-19 14:37:19.166606 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/_not-found/page-6eda385f9819e210.js
--rw-r--r--   0        0        0     1744 2024-05-22 22:55:21.612319 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/_not-found/page-a28cb215e1e35b93.js
--rw-r--r--   0        0        0     1840 2024-05-01 14:48:56.204570 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/_not-found-bee08356a690a144.js
--rw-r--r--   0        0        0      480 2024-05-02 18:20:15.926928 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/layout-0f23d4766ac3d9e3.js
--rw-r--r--   0        0        0      480 2024-05-22 22:55:21.613253 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/layout-15dece07a8c94bf7.js
--rw-r--r--   0        0        0      477 2024-05-01 14:48:56.206202 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/layout-f917f547d72d1629.js
--rw-r--r--   0        0        0    26631 2024-05-07 09:53:06.301663 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/page-0dc09429eb1650c3.js
--rw-r--r--   0        0        0    26688 2024-05-01 15:15:14.526938 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/page-0dcd9b5adc14930a.js
--rw-r--r--   0        0        0    27085 2024-05-18 14:34:34.750017 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/page-17df7cbc5c638eea.js
--rw-r--r--   0        0        0    28397 2024-05-19 14:37:19.164068 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/page-1e3dd5bf43f67704.js
--rw-r--r--   0        0        0    26619 2024-05-01 14:48:56.207662 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/page-4f1f75de895ef2e9.js
--rw-r--r--   0        0        0    28341 2024-05-19 14:30:39.203825 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/page-6a91493712bff557.js
--rw-r--r--   0        0        0    38617 2024-05-22 22:55:21.609767 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/page-91409c3b5a506bcd.js
--rw-r--r--   0        0        0    26640 2024-05-01 14:48:56.208488 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/page-cc11fa76e9925a25.js
--rw-r--r--   0        0        0    27859 2024-05-01 14:48:56.209652 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/page-facced18ab368811.js
--rw-r--r--   0        0        0  3613214 2024-05-22 22:55:21.608113 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/f2d0f643.3ca4096564deaa88.js
--rw-r--r--   0        0        0  3842147 2024-05-01 14:48:56.238679 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/f2d0f643.db7d448233298422.js
--rw-r--r--   0        0        0   172831 2024-05-19 14:37:19.170998 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/fd9d1056-3324b1349d932382.js
--rw-r--r--   0        0        0   172831 2024-05-22 22:55:21.618686 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/fd9d1056-c8a9c2618497583f.js
--rw-r--r--   0        0        0   163906 2024-05-01 14:48:56.242705 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/fd9d1056-e13d3c2807942cb7.js
--rw-r--r--   0        0        0   140171 2024-05-01 14:48:56.244603 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/framework-8883d1e9be70c3da.js
--rw-r--r--   0        0        0   140981 2024-05-22 22:55:21.619892 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/framework-aec844d2ccbe7592.js
--rw-r--r--   0        0        0   115325 2024-05-01 14:48:56.246881 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/main-01a7d75e7a6a7c98.js
--rw-r--r--   0        0        0   109895 2024-05-22 22:55:21.628299 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/main-0ba5df58c56b45df.js
--rw-r--r--   0        0        0      508 2024-05-01 14:48:56.248662 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/main-app-27650c6b197f0cd8.js
--rw-r--r--   0        0        0      462 2024-05-22 22:55:21.620477 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/main-app-e01e327631e02231.js
--rw-r--r--   0        0        0      325 2024-05-01 14:48:56.250189 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/pages/_app-1534f180665c857f.js
--rw-r--r--   0        0        0      280 2024-05-22 22:55:21.626892 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/pages/_app-6a626577ffa902a4.js
--rw-r--r--   0        0        0      247 2024-05-22 22:55:21.627407 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/pages/_error-1be831200e60c5c0.js
--rw-r--r--   0        0        0      247 2024-05-01 14:48:56.252577 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/pages/_error-b646007f40c4f0a8.js
--rw-r--r--   0        0        0    91381 2024-05-22 22:55:21.629227 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js
--rw-r--r--   0        0        0    91460 2024-05-01 14:48:56.253498 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0        0        0     3839 2024-05-22 22:55:21.619172 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/webpack-363c75f55b5f9b13.js
--rw-r--r--   0        0        0     4659 2024-05-01 14:48:56.254092 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/webpack-60a4426b837ea404.js
--rw-r--r--   0        0        0     3839 2024-05-19 14:37:19.174368 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/webpack-96cd9861806fb7cf.js
--rw-r--r--   0        0        0     3824 2024-05-07 09:53:06.309226 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/webpack-9c62b174fdbd129f.js
--rw-r--r--   0        0        0    28962 2024-05-07 09:53:06.287289 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/css/23cc4be46f2171d6.css
--rw-r--r--   0        0        0    29727 2024-05-19 14:37:19.156669 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/css/61a2a53c075c2fd0.css
--rw-r--r--   0        0        0    28962 2024-05-01 14:48:56.256127 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/css/64b8c25cc96a1f37.css
--rw-r--r--   0        0        0    29471 2024-05-18 14:34:34.740653 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/css/997199f83c4c280c.css
--rw-r--r--   0        0        0    31218 2024-05-22 22:55:21.600617 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/css/b9222cfa4e2b440e.css
--rw-r--r--   0        0        0      224 2024-05-18 14:34:34.738729 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/eZIQk-vV3uUUtBXOaqaJj/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-18 14:34:34.737263 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/eZIQk-vV3uUUtBXOaqaJj/_ssgManifest.js
--rw-r--r--   0        0        0      224 2024-05-01 14:48:56.256638 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/gTuZP6baQRuoAlSBQfJhW/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-01 14:48:56.256845 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/gTuZP6baQRuoAlSBQfJhW/_ssgManifest.js
--rw-r--r--   0        0        0      224 2024-05-02 18:20:15.928020 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/lbjNsPpWYZod25BysgHf4/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-02 18:20:15.928227 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/lbjNsPpWYZod25BysgHf4/_ssgManifest.js
--rw-r--r--   0        0        0      224 2024-05-01 14:48:56.257630 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/mBEYttyj_pgzUHdneL-73/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-01 14:48:56.257857 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/mBEYttyj_pgzUHdneL-73/_ssgManifest.js
--rw-r--r--   0        0        0    10496 2024-05-22 22:55:21.630811 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/media/05a31a2ca4975f99-s.woff2
--rw-r--r--   0        0        0    17612 2024-05-22 22:55:21.640081 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/media/513657b02c5c193f-s.woff2
--rw-r--r--   0        0        0    22524 2024-05-22 22:55:21.637219 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/media/51ed15f9841b9f9d-s.woff2
--rw-r--r--   0        0        0     9628 2024-05-22 22:55:21.630282 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/media/Oliver-Regular-400.365d360e.woff
--rw-r--r--   0        0        0    46552 2024-05-22 22:55:21.637840 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/media/c9a5bc6a7c948fb0-s.p.woff2
--rw-r--r--   0        0        0    80044 2024-05-22 22:55:21.638851 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/media/d6b16ce4a6175f26-s.woff2
--rw-r--r--   0        0        0    27316 2024-05-22 22:55:21.638369 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/media/ec159349637c90ad-s.woff2
--rw-r--r--   0        0        0    12768 2024-05-22 22:55:21.639422 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/media/fd4db3eb5472fc27-s.woff2
--rw-r--r--   0        0        0      224 2024-05-19 14:30:39.196700 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/w_YL5rdlxmN6WmZSxGr80/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-19 14:30:39.195960 clusterfun-0.5.0a7/clusterfun/frontend/_next/static/w_YL5rdlxmN6WmZSxGr80/_ssgManifest.js
--rw-r--r--   0        0        0     7406 2024-05-22 22:55:21.643406 clusterfun-0.5.0a7/clusterfun/frontend/favicon.ico
--rw-r--r--   0        0        0     9628 2024-05-22 22:55:21.646276 clusterfun-0.5.0a7/clusterfun/frontend/fonts/Oliver-Regular-400.woff
--rw-r--r--   0        0        0     5067 2024-05-22 22:55:21.646769 clusterfun-0.5.0a7/clusterfun/frontend/index.html
--rw-r--r--   0        0        0     2498 2024-05-22 22:55:21.648069 clusterfun-0.5.0a7/clusterfun/frontend/index.txt
--rw-r--r--   0        0        0     6654 2024-05-22 22:53:46.025636 clusterfun-0.5.0a7/clusterfun/main.py
--rw-r--r--   0        0        0        0 2024-04-28 22:32:09.895406 clusterfun-0.5.0a7/clusterfun/models/__init__.py
--rw-r--r--   0        0        0     3111 2024-04-28 22:32:09.895643 clusterfun-0.5.0a7/clusterfun/models/filter.py
--rw-r--r--   0        0        0     1159 2024-04-28 22:32:09.895855 clusterfun-0.5.0a7/clusterfun/models/media_indices.py
--rw-r--r--   0        0        0     1168 2024-05-22 22:53:46.028396 clusterfun-0.5.0a7/clusterfun/models/media_item.py
--rw-r--r--   0        0        0     8100 2024-05-03 13:14:27.292482 clusterfun-0.5.0a7/clusterfun/plot.py
--rw-r--r--   0        0        0     1591 2024-05-19 13:48:08.178126 clusterfun-0.5.0a7/clusterfun/plot_types/__init__.py
--rw-r--r--   0        0        0     3795 2024-05-19 13:49:56.505087 clusterfun-0.5.0a7/clusterfun/plot_types/bar_chart.py
--rw-r--r--   0        0        0     3257 2024-05-19 13:49:39.123145 clusterfun-0.5.0a7/clusterfun/plot_types/confusion_matrix.py
--rw-r--r--   0        0        0     1345 2024-05-22 22:53:46.030465 clusterfun-0.5.0a7/clusterfun/plot_types/grid.py
--rw-r--r--   0        0        0     4448 2024-05-19 13:50:18.186383 clusterfun-0.5.0a7/clusterfun/plot_types/histogram.py
--rw-r--r--   0        0        0     6210 2024-05-19 14:52:40.464275 clusterfun-0.5.0a7/clusterfun/plot_types/pie_chart.py
--rw-r--r--   0        0        0     1537 2024-05-19 13:51:00.708952 clusterfun-0.5.0a7/clusterfun/plot_types/scatter.py
--rw-r--r--   0        0        0     4362 2024-05-19 13:52:12.494079 clusterfun-0.5.0a7/clusterfun/plot_types/violin.py
--rw-r--r--   0        0        0     1721 2024-04-28 22:32:09.900538 clusterfun-0.5.0a7/clusterfun/serve_cli.py
--rw-r--r--   0        0        0        0 2024-04-28 22:32:09.900856 clusterfun-0.5.0a7/clusterfun/storage/__init__.py
--rw-r--r--   0        0        0      991 2024-05-09 22:09:16.226778 clusterfun-0.5.0a7/clusterfun/storage/client/__init__.py
--rw-r--r--   0        0        0     1249 2024-05-07 09:18:46.136998 clusterfun-0.5.0a7/clusterfun/storage/client/base.py
--rw-r--r--   0        0        0      800 2024-05-07 09:18:46.136720 clusterfun-0.5.0a7/clusterfun/storage/client/http.py
--rw-r--r--   0        0        0     1071 2024-05-07 09:18:46.140218 clusterfun-0.5.0a7/clusterfun/storage/client/local.py
--rw-r--r--   0        0        0     1680 2024-05-07 09:51:17.155237 clusterfun-0.5.0a7/clusterfun/storage/client/s3.py
--rw-r--r--   0        0        0     2238 2024-05-21 21:12:24.045790 clusterfun-0.5.0a7/clusterfun/storage/loader.py
--rw-r--r--   0        0        0        0 2024-04-28 22:32:09.902140 clusterfun-0.5.0a7/clusterfun/storage/local/__init__.py
--rw-r--r--   0        0        0     5772 2024-05-09 22:09:16.227345 clusterfun-0.5.0a7/clusterfun/storage/local/data.py
--rw-r--r--   0        0        0     4767 2024-05-02 18:20:15.931749 clusterfun-0.5.0a7/clusterfun/storage/local/helpers.py
--rw-r--r--   0        0        0     3952 2024-05-22 22:53:46.030861 clusterfun-0.5.0a7/clusterfun/storage/local/label_manager.py
--rw-r--r--   0        0        0     6238 2024-05-22 22:53:46.031674 clusterfun-0.5.0a7/clusterfun/storage/local/loader.py
--rw-r--r--   0        0        0     2853 2024-05-19 13:54:34.238130 clusterfun-0.5.0a7/clusterfun/storage/local/storer.py
--rw-r--r--   0        0        0     2629 2024-05-06 22:44:34.096055 clusterfun-0.5.0a7/clusterfun/storage/storer.py
--rw-r--r--   0        0        0     2258 2024-04-28 22:32:09.904443 clusterfun-0.5.0a7/clusterfun/validation.py
--rw-r--r--   0        0        0     1130 2024-05-22 22:56:29.270650 clusterfun-0.5.0a7/pyproject.toml
--rw-r--r--   0        0        0    10021 1970-01-01 00:00:00.000000 clusterfun-0.5.0a7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-28 22:32:09.819834 clusterfun-0.5.1a7/LICENSE
+-rw-r--r--   0        0        0     9280 2024-04-28 22:32:09.820288 clusterfun-0.5.1a7/README.md
+-rw-r--r--   0        0        0      660 2024-04-28 22:32:09.852017 clusterfun-0.5.1a7/clusterfun/__init__.py
+-rw-r--r--   0        0        0      970 2024-05-19 14:26:30.502142 clusterfun-0.5.1a7/clusterfun/app.py
+-rw-r--r--   0        0        0     2750 2024-05-22 22:53:46.023349 clusterfun-0.5.1a7/clusterfun/config.py
+-rw-r--r--   0        0        0      715 2024-04-28 22:32:09.852760 clusterfun-0.5.1a7/clusterfun/constants.py
+-rw-r--r--   0        0        0     6790 2024-05-22 22:55:21.594564 clusterfun-0.5.1a7/clusterfun/frontend/404.html
+-rw-r--r--   0        0        0      224 2024-05-02 18:20:15.920034 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/0L8U1RGbBQqzpAEgBP-4y/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-02 18:20:15.920441 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/0L8U1RGbBQqzpAEgBP-4y/_ssgManifest.js
+-rw-r--r--   0        0        0      224 2024-05-07 09:53:06.289880 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/0t2IpDcBx6FIaFpL5-DTX/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-07 09:53:06.288728 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/0t2IpDcBx6FIaFpL5-DTX/_ssgManifest.js
+-rw-r--r--   0        0        0      224 2024-05-01 14:48:56.190992 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/7K0stYTjLuE1ieiHwaOY8/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-01 14:48:56.191316 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/7K0stYTjLuE1ieiHwaOY8/_ssgManifest.js
+-rw-r--r--   0        0        0      224 2024-05-01 14:48:56.192076 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/9m8W0thtsOjMrVxSpss7G/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-01 14:48:56.192715 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/9m8W0thtsOjMrVxSpss7G/_ssgManifest.js
+-rw-r--r--   0        0        0      224 2024-05-02 18:20:15.921043 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/FajzyA8s2dBSB6nVAodLv/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-02 18:20:15.921298 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/FajzyA8s2dBSB6nVAodLv/_ssgManifest.js
+-rw-r--r--   0        0        0      224 2024-05-22 22:55:21.599225 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/P5xyy85ON_Ic7d-vfYKXs/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-22 22:55:21.598755 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/P5xyy85ON_Ic7d-vfYKXs/_ssgManifest.js
+-rw-r--r--   0        0        0      224 2024-05-19 14:37:19.186304 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/U2JWEnXogvGKNw9dZYznH/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-19 14:37:19.184257 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/U2JWEnXogvGKNw9dZYznH/_ssgManifest.js
+-rw-r--r--   0        0        0     8025 2024-05-01 14:48:56.193828 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/22.94ebc66962dcd0f8.js
+-rw-r--r--   0        0        0   121966 2024-05-19 14:37:19.168355 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/23-8126128752749016.js
+-rw-r--r--   0        0        0   121966 2024-05-22 22:55:21.621856 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/23-916fe2f1983668e3.js
+-rw-r--r--   0        0        0   110785 2024-05-01 14:48:56.198064 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/472-07a7dd51a787971b.js
+-rw-r--r--   0        0        0   143320 2024-05-01 14:48:56.199462 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/483-2d99a375fdcaeaa9.js
+-rw-r--r--   0        0        0   131700 2024-05-02 18:20:15.926209 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/500-9855c0cda36bb0be.js
+-rw-r--r--   0        0        0   131700 2024-05-07 09:53:06.297351 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/500-9beb637c2f8db305.js
+-rw-r--r--   0        0        0   146876 2024-05-22 22:55:21.627851 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/771-1510a54548bf26b3.js
+-rw-r--r--   0        0        0     7388 2024-05-22 22:55:21.605280 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/8.d9282dffb5cd6834.js
+-rw-r--r--   0        0        0   134273 2024-05-19 14:37:19.171903 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/86-fdf3fe7d49e1a681.js
+-rw-r--r--   0        0        0     7683 2024-05-22 22:55:21.621352 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/870fdd6f-080da6c9b87ec5a2.js
+-rw-r--r--   0        0        0     4290 2024-05-18 14:34:34.764454 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/870fdd6f-4049d31c55f7218c.js
+-rw-r--r--   0        0        0     4290 2024-05-01 14:48:56.203293 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/870fdd6f-51765f2c6413dd54.js
+-rw-r--r--   0        0        0     5079 2024-05-19 14:37:19.173787 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/870fdd6f-728b0ab9f208053f.js
+-rw-r--r--   0        0        0     1744 2024-05-19 14:37:19.166606 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/_not-found/page-6eda385f9819e210.js
+-rw-r--r--   0        0        0     1744 2024-05-22 22:55:21.612319 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/_not-found/page-a28cb215e1e35b93.js
+-rw-r--r--   0        0        0     1840 2024-05-01 14:48:56.204570 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/_not-found-bee08356a690a144.js
+-rw-r--r--   0        0        0      480 2024-05-02 18:20:15.926928 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/layout-0f23d4766ac3d9e3.js
+-rw-r--r--   0        0        0      480 2024-05-22 22:55:21.613253 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/layout-15dece07a8c94bf7.js
+-rw-r--r--   0        0        0      477 2024-05-01 14:48:56.206202 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/layout-f917f547d72d1629.js
+-rw-r--r--   0        0        0    26631 2024-05-07 09:53:06.301663 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/page-0dc09429eb1650c3.js
+-rw-r--r--   0        0        0    26688 2024-05-01 15:15:14.526938 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/page-0dcd9b5adc14930a.js
+-rw-r--r--   0        0        0    27085 2024-05-18 14:34:34.750017 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/page-17df7cbc5c638eea.js
+-rw-r--r--   0        0        0    28397 2024-05-19 14:37:19.164068 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/page-1e3dd5bf43f67704.js
+-rw-r--r--   0        0        0    26619 2024-05-01 14:48:56.207662 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/page-4f1f75de895ef2e9.js
+-rw-r--r--   0        0        0    28341 2024-05-19 14:30:39.203825 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/page-6a91493712bff557.js
+-rw-r--r--   0        0        0    38617 2024-05-22 22:55:21.609767 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/page-91409c3b5a506bcd.js
+-rw-r--r--   0        0        0    26640 2024-05-01 14:48:56.208488 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/page-cc11fa76e9925a25.js
+-rw-r--r--   0        0        0    27859 2024-05-01 14:48:56.209652 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/page-facced18ab368811.js
+-rw-r--r--   0        0        0  3613214 2024-05-22 22:55:21.608113 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/f2d0f643.3ca4096564deaa88.js
+-rw-r--r--   0        0        0  3842147 2024-05-01 14:48:56.238679 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/f2d0f643.db7d448233298422.js
+-rw-r--r--   0        0        0   172831 2024-05-19 14:37:19.170998 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/fd9d1056-3324b1349d932382.js
+-rw-r--r--   0        0        0   172831 2024-05-22 22:55:21.618686 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/fd9d1056-c8a9c2618497583f.js
+-rw-r--r--   0        0        0   163906 2024-05-01 14:48:56.242705 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/fd9d1056-e13d3c2807942cb7.js
+-rw-r--r--   0        0        0   140171 2024-05-01 14:48:56.244603 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/framework-8883d1e9be70c3da.js
+-rw-r--r--   0        0        0   140981 2024-05-22 22:55:21.619892 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/framework-aec844d2ccbe7592.js
+-rw-r--r--   0        0        0   115325 2024-05-01 14:48:56.246881 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/main-01a7d75e7a6a7c98.js
+-rw-r--r--   0        0        0   109895 2024-05-22 22:55:21.628299 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/main-0ba5df58c56b45df.js
+-rw-r--r--   0        0        0      508 2024-05-01 14:48:56.248662 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/main-app-27650c6b197f0cd8.js
+-rw-r--r--   0        0        0      462 2024-05-22 22:55:21.620477 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/main-app-e01e327631e02231.js
+-rw-r--r--   0        0        0      325 2024-05-01 14:48:56.250189 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/pages/_app-1534f180665c857f.js
+-rw-r--r--   0        0        0      280 2024-05-22 22:55:21.626892 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/pages/_app-6a626577ffa902a4.js
+-rw-r--r--   0        0        0      247 2024-05-22 22:55:21.627407 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/pages/_error-1be831200e60c5c0.js
+-rw-r--r--   0        0        0      247 2024-05-01 14:48:56.252577 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/pages/_error-b646007f40c4f0a8.js
+-rw-r--r--   0        0        0    91381 2024-05-22 22:55:21.629227 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js
+-rw-r--r--   0        0        0    91460 2024-05-01 14:48:56.253498 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0        0        0     3839 2024-05-22 22:55:21.619172 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/webpack-363c75f55b5f9b13.js
+-rw-r--r--   0        0        0     4659 2024-05-01 14:48:56.254092 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/webpack-60a4426b837ea404.js
+-rw-r--r--   0        0        0     3839 2024-05-19 14:37:19.174368 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/webpack-96cd9861806fb7cf.js
+-rw-r--r--   0        0        0     3824 2024-05-07 09:53:06.309226 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/webpack-9c62b174fdbd129f.js
+-rw-r--r--   0        0        0    28962 2024-05-07 09:53:06.287289 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/css/23cc4be46f2171d6.css
+-rw-r--r--   0        0        0    29727 2024-05-19 14:37:19.156669 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/css/61a2a53c075c2fd0.css
+-rw-r--r--   0        0        0    28962 2024-05-01 14:48:56.256127 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/css/64b8c25cc96a1f37.css
+-rw-r--r--   0        0        0    29471 2024-05-18 14:34:34.740653 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/css/997199f83c4c280c.css
+-rw-r--r--   0        0        0    31218 2024-05-22 22:55:21.600617 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/css/b9222cfa4e2b440e.css
+-rw-r--r--   0        0        0      224 2024-05-18 14:34:34.738729 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/eZIQk-vV3uUUtBXOaqaJj/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-18 14:34:34.737263 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/eZIQk-vV3uUUtBXOaqaJj/_ssgManifest.js
+-rw-r--r--   0        0        0      224 2024-05-01 14:48:56.256638 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/gTuZP6baQRuoAlSBQfJhW/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-01 14:48:56.256845 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/gTuZP6baQRuoAlSBQfJhW/_ssgManifest.js
+-rw-r--r--   0        0        0      224 2024-05-02 18:20:15.928020 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/lbjNsPpWYZod25BysgHf4/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-02 18:20:15.928227 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/lbjNsPpWYZod25BysgHf4/_ssgManifest.js
+-rw-r--r--   0        0        0      224 2024-05-01 14:48:56.257630 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/mBEYttyj_pgzUHdneL-73/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-01 14:48:56.257857 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/mBEYttyj_pgzUHdneL-73/_ssgManifest.js
+-rw-r--r--   0        0        0    10496 2024-05-22 22:55:21.630811 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/media/05a31a2ca4975f99-s.woff2
+-rw-r--r--   0        0        0    17612 2024-05-22 22:55:21.640081 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/media/513657b02c5c193f-s.woff2
+-rw-r--r--   0        0        0    22524 2024-05-22 22:55:21.637219 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/media/51ed15f9841b9f9d-s.woff2
+-rw-r--r--   0        0        0     9628 2024-05-22 22:55:21.630282 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/media/Oliver-Regular-400.365d360e.woff
+-rw-r--r--   0        0        0    46552 2024-05-22 22:55:21.637840 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/media/c9a5bc6a7c948fb0-s.p.woff2
+-rw-r--r--   0        0        0    80044 2024-05-22 22:55:21.638851 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/media/d6b16ce4a6175f26-s.woff2
+-rw-r--r--   0        0        0    27316 2024-05-22 22:55:21.638369 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/media/ec159349637c90ad-s.woff2
+-rw-r--r--   0        0        0    12768 2024-05-22 22:55:21.639422 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/media/fd4db3eb5472fc27-s.woff2
+-rw-r--r--   0        0        0      224 2024-05-19 14:30:39.196700 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/w_YL5rdlxmN6WmZSxGr80/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-19 14:30:39.195960 clusterfun-0.5.1a7/clusterfun/frontend/_next/static/w_YL5rdlxmN6WmZSxGr80/_ssgManifest.js
+-rw-r--r--   0        0        0     7406 2024-05-22 22:55:21.643406 clusterfun-0.5.1a7/clusterfun/frontend/favicon.ico
+-rw-r--r--   0        0        0     9628 2024-05-22 22:55:21.646276 clusterfun-0.5.1a7/clusterfun/frontend/fonts/Oliver-Regular-400.woff
+-rw-r--r--   0        0        0     5067 2024-05-22 22:55:21.646769 clusterfun-0.5.1a7/clusterfun/frontend/index.html
+-rw-r--r--   0        0        0     2498 2024-05-22 22:55:21.648069 clusterfun-0.5.1a7/clusterfun/frontend/index.txt
+-rw-r--r--   0        0        0     6654 2024-05-22 22:53:46.025636 clusterfun-0.5.1a7/clusterfun/main.py
+-rw-r--r--   0        0        0        0 2024-04-28 22:32:09.895406 clusterfun-0.5.1a7/clusterfun/models/__init__.py
+-rw-r--r--   0        0        0     3111 2024-04-28 22:32:09.895643 clusterfun-0.5.1a7/clusterfun/models/filter.py
+-rw-r--r--   0        0        0     1159 2024-04-28 22:32:09.895855 clusterfun-0.5.1a7/clusterfun/models/media_indices.py
+-rw-r--r--   0        0        0     1168 2024-05-22 22:53:46.028396 clusterfun-0.5.1a7/clusterfun/models/media_item.py
+-rw-r--r--   0        0        0     8221 2024-05-23 10:03:14.382775 clusterfun-0.5.1a7/clusterfun/plot.py
+-rw-r--r--   0        0        0     1591 2024-05-19 13:48:08.178126 clusterfun-0.5.1a7/clusterfun/plot_types/__init__.py
+-rw-r--r--   0        0        0     3795 2024-05-19 13:49:56.505087 clusterfun-0.5.1a7/clusterfun/plot_types/bar_chart.py
+-rw-r--r--   0        0        0     3257 2024-05-19 13:49:39.123145 clusterfun-0.5.1a7/clusterfun/plot_types/confusion_matrix.py
+-rw-r--r--   0        0        0     1345 2024-05-22 22:53:46.030465 clusterfun-0.5.1a7/clusterfun/plot_types/grid.py
+-rw-r--r--   0        0        0     4448 2024-05-19 13:50:18.186383 clusterfun-0.5.1a7/clusterfun/plot_types/histogram.py
+-rw-r--r--   0        0        0     6210 2024-05-19 14:52:40.464275 clusterfun-0.5.1a7/clusterfun/plot_types/pie_chart.py
+-rw-r--r--   0        0        0     1537 2024-05-19 13:51:00.708952 clusterfun-0.5.1a7/clusterfun/plot_types/scatter.py
+-rw-r--r--   0        0        0     4362 2024-05-19 13:52:12.494079 clusterfun-0.5.1a7/clusterfun/plot_types/violin.py
+-rw-r--r--   0        0        0     1721 2024-04-28 22:32:09.900538 clusterfun-0.5.1a7/clusterfun/serve_cli.py
+-rw-r--r--   0        0        0        0 2024-04-28 22:32:09.900856 clusterfun-0.5.1a7/clusterfun/storage/__init__.py
+-rw-r--r--   0        0        0      991 2024-05-23 10:03:06.695716 clusterfun-0.5.1a7/clusterfun/storage/client/__init__.py
+-rw-r--r--   0        0        0     1249 2024-05-07 09:18:46.136998 clusterfun-0.5.1a7/clusterfun/storage/client/base.py
+-rw-r--r--   0        0        0      800 2024-05-07 09:18:46.136720 clusterfun-0.5.1a7/clusterfun/storage/client/http.py
+-rw-r--r--   0        0        0     1071 2024-05-07 09:18:46.140218 clusterfun-0.5.1a7/clusterfun/storage/client/local.py
+-rw-r--r--   0        0        0     1680 2024-05-07 09:51:17.155237 clusterfun-0.5.1a7/clusterfun/storage/client/s3.py
+-rw-r--r--   0        0        0     2238 2024-05-21 21:12:24.045790 clusterfun-0.5.1a7/clusterfun/storage/loader.py
+-rw-r--r--   0        0        0        0 2024-04-28 22:32:09.902140 clusterfun-0.5.1a7/clusterfun/storage/local/__init__.py
+-rw-r--r--   0        0        0     5772 2024-05-09 22:09:16.227345 clusterfun-0.5.1a7/clusterfun/storage/local/data.py
+-rw-r--r--   0        0        0     4767 2024-05-02 18:20:15.931749 clusterfun-0.5.1a7/clusterfun/storage/local/helpers.py
+-rw-r--r--   0        0        0     3952 2024-05-22 22:53:46.030861 clusterfun-0.5.1a7/clusterfun/storage/local/label_manager.py
+-rw-r--r--   0        0        0     6256 2024-05-23 10:03:31.338411 clusterfun-0.5.1a7/clusterfun/storage/local/loader.py
+-rw-r--r--   0        0        0     2853 2024-05-19 13:54:34.238130 clusterfun-0.5.1a7/clusterfun/storage/local/storer.py
+-rw-r--r--   0        0        0     2629 2024-05-06 22:44:34.096055 clusterfun-0.5.1a7/clusterfun/storage/storer.py
+-rw-r--r--   0        0        0     2258 2024-04-28 22:32:09.904443 clusterfun-0.5.1a7/clusterfun/validation.py
+-rw-r--r--   0        0        0     1130 2024-05-23 10:05:52.881284 clusterfun-0.5.1a7/pyproject.toml
+-rw-r--r--   0        0        0    10021 1970-01-01 00:00:00.000000 clusterfun-0.5.1a7/PKG-INFO
```

### Comparing `clusterfun-0.5.0a7/LICENSE` & `clusterfun-0.5.1a7/LICENSE`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/README.md` & `clusterfun-0.5.1a7/README.md`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/__init__.py` & `clusterfun-0.5.1a7/clusterfun/__init__.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/app.py` & `clusterfun-0.5.1a7/clusterfun/app.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/config.py` & `clusterfun-0.5.1a7/clusterfun/config.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/constants.py` & `clusterfun-0.5.1a7/clusterfun/constants.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/404.html` & `clusterfun-0.5.1a7/clusterfun/frontend/404.html`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/22.94ebc66962dcd0f8.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/22.94ebc66962dcd0f8.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/23-8126128752749016.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/23-8126128752749016.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/23-916fe2f1983668e3.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/23-916fe2f1983668e3.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/472-07a7dd51a787971b.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/472-07a7dd51a787971b.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/483-2d99a375fdcaeaa9.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/483-2d99a375fdcaeaa9.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/500-9855c0cda36bb0be.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/500-9855c0cda36bb0be.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/500-9beb637c2f8db305.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/500-9beb637c2f8db305.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/771-1510a54548bf26b3.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/771-1510a54548bf26b3.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/8.d9282dffb5cd6834.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/8.d9282dffb5cd6834.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/86-fdf3fe7d49e1a681.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/86-fdf3fe7d49e1a681.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/870fdd6f-080da6c9b87ec5a2.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/870fdd6f-080da6c9b87ec5a2.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/870fdd6f-4049d31c55f7218c.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/870fdd6f-4049d31c55f7218c.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/870fdd6f-51765f2c6413dd54.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/870fdd6f-51765f2c6413dd54.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/870fdd6f-728b0ab9f208053f.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/870fdd6f-728b0ab9f208053f.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/_not-found/page-6eda385f9819e210.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/_not-found/page-6eda385f9819e210.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/_not-found/page-a28cb215e1e35b93.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/_not-found/page-a28cb215e1e35b93.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/_not-found-bee08356a690a144.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/_not-found-bee08356a690a144.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/page-0dc09429eb1650c3.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/page-0dc09429eb1650c3.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/page-0dcd9b5adc14930a.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/page-0dcd9b5adc14930a.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/page-17df7cbc5c638eea.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/page-17df7cbc5c638eea.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/page-1e3dd5bf43f67704.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/page-1e3dd5bf43f67704.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/page-4f1f75de895ef2e9.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/page-4f1f75de895ef2e9.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/page-6a91493712bff557.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/page-6a91493712bff557.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/page-91409c3b5a506bcd.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/page-91409c3b5a506bcd.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/page-cc11fa76e9925a25.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/page-cc11fa76e9925a25.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/app/page-facced18ab368811.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/app/page-facced18ab368811.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/f2d0f643.3ca4096564deaa88.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/f2d0f643.3ca4096564deaa88.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/f2d0f643.db7d448233298422.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/f2d0f643.db7d448233298422.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/fd9d1056-3324b1349d932382.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/fd9d1056-3324b1349d932382.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/fd9d1056-c8a9c2618497583f.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/fd9d1056-c8a9c2618497583f.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/fd9d1056-e13d3c2807942cb7.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/fd9d1056-e13d3c2807942cb7.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/framework-8883d1e9be70c3da.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/framework-8883d1e9be70c3da.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/framework-aec844d2ccbe7592.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/framework-aec844d2ccbe7592.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/main-01a7d75e7a6a7c98.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/main-01a7d75e7a6a7c98.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/main-0ba5df58c56b45df.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/main-0ba5df58c56b45df.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/webpack-363c75f55b5f9b13.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/webpack-363c75f55b5f9b13.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/webpack-60a4426b837ea404.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/webpack-60a4426b837ea404.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/webpack-96cd9861806fb7cf.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/webpack-96cd9861806fb7cf.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/chunks/webpack-9c62b174fdbd129f.js` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/chunks/webpack-9c62b174fdbd129f.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/css/23cc4be46f2171d6.css` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/css/23cc4be46f2171d6.css`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/css/61a2a53c075c2fd0.css` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/css/61a2a53c075c2fd0.css`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/css/64b8c25cc96a1f37.css` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/css/64b8c25cc96a1f37.css`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/css/997199f83c4c280c.css` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/css/997199f83c4c280c.css`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/css/b9222cfa4e2b440e.css` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/css/b9222cfa4e2b440e.css`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/media/05a31a2ca4975f99-s.woff2` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/media/05a31a2ca4975f99-s.woff2`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/media/513657b02c5c193f-s.woff2` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/media/513657b02c5c193f-s.woff2`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/media/51ed15f9841b9f9d-s.woff2` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/media/51ed15f9841b9f9d-s.woff2`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/media/Oliver-Regular-400.365d360e.woff` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/media/Oliver-Regular-400.365d360e.woff`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/media/c9a5bc6a7c948fb0-s.p.woff2` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/media/c9a5bc6a7c948fb0-s.p.woff2`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/media/d6b16ce4a6175f26-s.woff2` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/media/d6b16ce4a6175f26-s.woff2`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/media/ec159349637c90ad-s.woff2` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/media/ec159349637c90ad-s.woff2`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/_next/static/media/fd4db3eb5472fc27-s.woff2` & `clusterfun-0.5.1a7/clusterfun/frontend/_next/static/media/fd4db3eb5472fc27-s.woff2`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/favicon.ico` & `clusterfun-0.5.1a7/clusterfun/frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/fonts/Oliver-Regular-400.woff` & `clusterfun-0.5.1a7/clusterfun/frontend/fonts/Oliver-Regular-400.woff`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/index.html` & `clusterfun-0.5.1a7/clusterfun/frontend/index.html`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/frontend/index.txt` & `clusterfun-0.5.1a7/clusterfun/frontend/index.txt`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/main.py` & `clusterfun-0.5.1a7/clusterfun/main.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/models/filter.py` & `clusterfun-0.5.1a7/clusterfun/models/filter.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/models/media_indices.py` & `clusterfun-0.5.1a7/clusterfun/models/media_indices.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/models/media_item.py` & `clusterfun-0.5.1a7/clusterfun/models/media_item.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/plot.py` & `clusterfun-0.5.1a7/clusterfun/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,16 @@
         """
         # copy dataframe to not change original input
         df = df.copy()
         uuid = str(uuid4())
         if not str(df[cfg.media].iloc[0]).startswith("http") and not str(df[cfg.media].iloc[0]).startswith("s3://"):
             # assume all media paths are local and replace with /media
             common_media_path = os.path.commonpath(df[cfg.media].tolist())
+            if os.path.isfile(common_media_path):
+                common_media_path = os.path.dirname(common_media_path)
             # store common media path in config
             cfg.common_media_path = common_media_path
             df[cfg.media] = df[cfg.media].astype(str).str.replace(str(common_media_path), "/media")
             APP.mount("/media", StaticFiles(directory=common_media_path), name="media")
         LocalStorer().save(uuid, df, cfg)
         return cls(uuid, df.to_dict(), cfg)
```

### Comparing `clusterfun-0.5.0a7/clusterfun/plot_types/__init__.py` & `clusterfun-0.5.1a7/clusterfun/plot_types/__init__.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/plot_types/bar_chart.py` & `clusterfun-0.5.1a7/clusterfun/plot_types/bar_chart.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/plot_types/confusion_matrix.py` & `clusterfun-0.5.1a7/clusterfun/plot_types/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/plot_types/grid.py` & `clusterfun-0.5.1a7/clusterfun/plot_types/grid.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/plot_types/histogram.py` & `clusterfun-0.5.1a7/clusterfun/plot_types/histogram.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/plot_types/pie_chart.py` & `clusterfun-0.5.1a7/clusterfun/plot_types/pie_chart.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/plot_types/scatter.py` & `clusterfun-0.5.1a7/clusterfun/plot_types/scatter.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/plot_types/violin.py` & `clusterfun-0.5.1a7/clusterfun/plot_types/violin.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/serve_cli.py` & `clusterfun-0.5.1a7/clusterfun/serve_cli.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/storage/client/__init__.py` & `clusterfun-0.5.1a7/clusterfun/storage/client/__init__.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/storage/client/base.py` & `clusterfun-0.5.1a7/clusterfun/storage/client/base.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/storage/client/http.py` & `clusterfun-0.5.1a7/clusterfun/storage/client/http.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/storage/client/local.py` & `clusterfun-0.5.1a7/clusterfun/storage/client/local.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/storage/client/s3.py` & `clusterfun-0.5.1a7/clusterfun/storage/client/s3.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/storage/loader.py` & `clusterfun-0.5.1a7/clusterfun/storage/loader.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/storage/local/data.py` & `clusterfun-0.5.1a7/clusterfun/storage/local/data.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/storage/local/helpers.py` & `clusterfun-0.5.1a7/clusterfun/storage/local/helpers.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/storage/local/label_manager.py` & `clusterfun-0.5.1a7/clusterfun/storage/local/label_manager.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/storage/local/loader.py` & `clusterfun-0.5.1a7/clusterfun/storage/local/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,24 +93,23 @@
             Determines what to query
 
         Returns
         -------
         List[MediaItem]
             List of queried items
         """
-        con, config = None, None
+        con, config = None, self.load_config()
         if media_indices.filters:
             con = sqlite3.connect(self.db_path, check_same_thread=False)
-            config = self.load_config()
         query = get_media_query(media_indices, config=config, con=con)
         result = run_query(self.db_path, query)
         items = []
         labels = self.label_manager.read_labels()
         for item in result:
-            src, height, width = load_media(item[1])
+            src, height, width = load_media(item[1], common_media_path=config.common_media_path)
             labels_item = None
             if str(item[0]) in labels:
                 labels_item = labels[str(item[0])]
             item = MediaItem(
                 index=item[0], src=src, height=height, width=width, information=list(item[2:]), labels=labels_item
             )
             items.append(item)
```

### Comparing `clusterfun-0.5.0a7/clusterfun/storage/local/storer.py` & `clusterfun-0.5.1a7/clusterfun/storage/local/storer.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/storage/storer.py` & `clusterfun-0.5.1a7/clusterfun/storage/storer.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/clusterfun/validation.py` & `clusterfun-0.5.1a7/clusterfun/validation.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.5.0a7/pyproject.toml` & `clusterfun-0.5.1a7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clusterfun"
-version = "0.5.0a7"
+version = "0.5.1a7"
 description = "Clusterfun - a plotting library to inspect data"
 authors = ["Jochem Gietema <jochem@giete.ma>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 pandas = "^2.0.0"
```

### Comparing `clusterfun-0.5.0a7/PKG-INFO` & `clusterfun-0.5.1a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clusterfun
-Version: 0.5.0a7
+Version: 0.5.1a7
 Summary: Clusterfun - a plotting library to inspect data
 Author: Jochem Gietema
 Author-email: jochem@giete.ma
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

