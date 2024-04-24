# Comparing `tmp/ships-1.2.8.tar.gz` & `tmp/ships-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ships-1.2.8.tar", max compression
+gzip compressed data, was "ships-1.3.8.tar", max compression
```

## Comparing `ships-1.2.8.tar` & `ships-1.3.8.tar`

### file list

```diff
@@ -1,454 +1,458 @@
--rw-r--r--   0        0        0      104 2024-03-30 17:23:39.109806 ships-1.2.8/fields/gardens/ships/AMLI/AMLI.S.HTML
--rw-r--r--   0        0        0       61 2024-02-15 19:38:33.618784 ships-1.2.8/fields/gardens/ships/AMLI/LLM/LLM.S.HTML
--rw-r--r--   0        0        0       44 2024-02-15 19:38:43.658669 ships-1.2.8/fields/gardens/ships/Search/Search.s.HTML
--rw-r--r--   0        0        0     1008 2024-02-15 04:11:24.069788 ships-1.2.8/fields/gardens/ships/__init__.py
--rw-r--r--   0        0        0      547 2024-02-15 04:21:26.722722 ships-1.2.8/fields/gardens/ships/_clique/__init__.py
--rw-r--r--   0        0        0     1004 2024-02-15 04:21:33.042649 ships-1.2.8/fields/gardens/ships/_clique/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      173 2023-12-16 19:52:14.770884 ships-1.2.8/fields/gardens/ships/_license/license.s.HTML
--rw-r--r--   0        0        0    37279 2023-12-01 20:51:04.310266 ships-1.2.8/fields/gardens/ships/_license/licenses/gpl-3.0-standalone.html
--rw-r--r--   0        0        0    69632 2024-01-23 00:08:48.421730 ships-1.2.8/fields/gardens/ships/_status/.coverage
--rw-r--r--   0        0        0  1144202 2024-04-17 00:30:30.996234 ships-1.2.8/fields/gardens/ships/_status/DB/records.json
--rw-r--r--   0        0        0       27 2024-01-23 00:04:12.188823 ships-1.2.8/fields/gardens/ships/_status/coverage_report/.gitignore
--rw-r--r--   0        0        0    21865 2024-01-23 00:08:28.865949 ships-1.2.8/fields/gardens/ships/_status/coverage_report/coverage_html.js
--rw-r--r--   0        0        0    49384 2024-01-23 00:08:28.743950 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_45774dabac2a4451___init___py.html
--rw-r--r--   0        0        0    48035 2024-01-23 00:04:11.398832 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad___init___py.html
--rw-r--r--   0        0        0   160908 2024-01-23 00:04:11.422832 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__cell_widths_py.html
--rw-r--r--   0        0        0  1010994 2024-01-23 00:04:11.580830 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__emoji_codes_py.html
--rw-r--r--   0        0        0    14114 2024-01-23 00:04:11.586830 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__emoji_replace_py.html
--rw-r--r--   0        0        0    18535 2024-01-23 00:04:11.588830 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__export_format_py.html
--rw-r--r--   0        0        0    10425 2024-01-23 00:04:11.589830 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__fileno_py.html
--rw-r--r--   0        0        0    33320 2024-01-23 00:04:11.594830 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__log_render_py.html
--rw-r--r--   0        0        0    16305 2024-01-23 00:04:11.597830 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__loop_py.html
--rw-r--r--   0        0        0    22576 2024-01-23 00:04:11.600830 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__null_file_py.html
--rw-r--r--   0        0        0   108791 2024-01-23 00:04:11.616830 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__palettes_py.html
--rw-r--r--   0        0        0     8412 2024-01-23 00:04:11.618830 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__pick_py.html
--rw-r--r--   0        0        0    48386 2024-01-23 00:04:11.625830 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__ratio_py.html
--rw-r--r--   0        0        0    29373 2024-01-23 00:04:11.629830 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__wrap_py.html
--rw-r--r--   0        0        0    12484 2024-01-23 00:04:11.631830 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_abc_py.html
--rw-r--r--   0        0        0    91280 2024-01-23 00:04:11.655829 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_align_py.html
--rw-r--r--   0        0        0   112963 2024-01-23 00:04:11.669829 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_box_py.html
--rw-r--r--   0        0        0    47077 2024-01-23 00:04:11.677829 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_cells_py.html
--rw-r--r--   0        0        0   176081 2024-01-23 00:04:11.702829 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_color_py.html
--rw-r--r--   0        0        0    13311 2024-01-23 00:04:11.705829 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_color_triplet_py.html
--rw-r--r--   0        0        0   717904 2024-01-23 00:04:11.818827 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_console_py.html
--rw-r--r--   0        0        0    15230 2024-01-23 00:04:11.823828 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_constrain_py.html
--rw-r--r--   0        0        0    54307 2024-01-23 00:04:11.832827 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_containers_py.html
--rw-r--r--   0        0        0    62602 2024-01-23 00:04:11.841827 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_control_py.html
--rw-r--r--   0        0        0    80963 2024-01-23 00:04:11.853827 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_default_styles_py.html
--rw-r--r--   0        0        0    28704 2024-01-23 00:04:11.858827 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_emoji_py.html
--rw-r--r--   0        0        0    11215 2024-01-23 00:04:11.859827 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_errors_py.html
--rw-r--r--   0        0        0    60921 2024-01-23 00:04:11.866827 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_highlighter_py.html
--rw-r--r--   0        0        0    41115 2024-01-23 00:04:11.872827 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_json_py.html
--rw-r--r--   0        0        0    34765 2024-01-23 00:04:11.877827 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_jupyter_py.html
--rw-r--r--   0        0        0    72977 2024-01-23 00:04:11.888827 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_markup_py.html
--rw-r--r--   0        0        0    43367 2024-01-23 00:04:11.894827 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_measure_py.html
--rw-r--r--   0        0        0    46862 2024-01-23 00:04:11.901827 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_padding_py.html
--rw-r--r--   0        0        0    12954 2024-01-23 00:04:11.903827 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_pager_py.html
--rw-r--r--   0        0        0    35002 2024-01-23 00:04:11.908826 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_palette_py.html
--rw-r--r--   0        0        0    92571 2024-01-23 00:04:11.921826 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_panel_py.html
--rw-r--r--   0        0        0   279872 2024-01-23 00:04:11.960826 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_pretty_py.html
--rw-r--r--   0        0        0    15360 2024-01-23 00:04:11.963826 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_protocol_py.html
--rw-r--r--   0        0        0     6679 2024-01-23 00:04:11.964826 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_region_py.html
--rw-r--r--   0        0        0    47741 2024-01-23 00:04:11.972826 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_repr_py.html
--rw-r--r--   0        0        0    28545 2024-01-23 00:04:11.976826 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_scope_py.html
--rw-r--r--   0        0        0    18971 2024-01-23 00:04:11.978826 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_screen_py.html
--rw-r--r--   0        0        0   197532 2024-01-23 00:04:12.016825 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_segment_py.html
--rw-r--r--   0        0        0   232858 2024-01-23 00:04:12.050825 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_style_py.html
--rw-r--r--   0        0        0    15742 2024-01-23 00:04:12.053825 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_styled_py.html
--rw-r--r--   0        0        0   291082 2024-01-23 00:04:12.093824 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_table_py.html
--rw-r--r--   0        0        0    49301 2024-01-23 00:04:12.101824 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_terminal_theme_py.html
--rw-r--r--   0        0        0   384696 2024-01-23 00:04:12.168824 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_text_py.html
--rw-r--r--   0        0        0    36139 2024-01-23 00:04:12.183823 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_theme_py.html
--rw-r--r--   0        0        0     5766 2024-01-23 00:04:12.185824 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_themes_py.html
--rw-r--r--   0        0        0    13616 2024-01-23 00:04:11.284834 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_9c84d462c231d294_exceptions_py.html
--rw-r--r--   0        0        0   113380 2024-01-23 00:04:11.299833 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_9c84d462c231d294_expect_py.html
--rw-r--r--   0        0        0   227312 2024-01-23 00:08:28.770950 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_9c84d462c231d294_pty_spawn_py.html
--rw-r--r--   0        0        0   144953 2024-01-23 00:08:28.799950 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_9c84d462c231d294_spawnbase_py.html
--rw-r--r--   0        0        0    52548 2024-01-23 00:04:11.363833 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_9c84d462c231d294_utils_py.html
--rw-r--r--   0        0        0   228779 2024-01-23 00:08:28.829949 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_acd758f7e5b0fd78_ptyprocess_py.html
--rw-r--r--   0        0        0    48168 2024-01-23 00:05:49.589733 ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_f85661004356945c___init___py.html
--rw-r--r--   0        0        0     1732 2024-01-23 00:08:28.865949 ships-1.2.8/fields/gardens/ships/_status/coverage_report/favicon_32.png
--rw-r--r--   0        0        0    26478 2024-01-23 00:08:28.864949 ships-1.2.8/fields/gardens/ships/_status/coverage_report/index.html
--rw-r--r--   0        0        0     9004 2024-01-23 00:08:28.865949 ships-1.2.8/fields/gardens/ships/_status/coverage_report/keybd_closed.png
--rw-r--r--   0        0        0     9003 2024-01-23 00:08:28.865949 ships-1.2.8/fields/gardens/ships/_status/coverage_report/keybd_open.png
--rw-r--r--   0        0        0    17880 2024-01-23 00:08:28.865949 ships-1.2.8/fields/gardens/ships/_status/coverage_report/status.json
--rw-r--r--   0        0        0    12406 2024-01-23 00:08:28.865949 ships-1.2.8/fields/gardens/ships/_status/coverage_report/style.css
--rw-r--r--   0        0        0      198 2024-01-23 03:57:34.614884 ships-1.2.8/fields/gardens/ships/_status/ports.py
--rw-r--r--   0        0        0      994 2024-04-17 00:26:54.579284 ships-1.2.8/fields/gardens/ships/_status/status.proc.py
--rw-r--r--   0        0        0       77 2023-11-22 19:02:46.200327 ships-1.2.8/fields/gardens/ships/business/business.s.HTML
--rw-r--r--   0        0        0       65 2023-11-22 19:10:51.771905 ships-1.2.8/fields/gardens/ships/business/decorators/decorators.r.HTML
--rw-r--r--   0        0        0      747 2023-11-22 19:15:14.376973 ships-1.2.8/fields/gardens/ships/business/decorators/examples/example_1.py
--rw-r--r--   0        0        0       93 2023-11-22 19:09:40.879696 ships-1.2.8/fields/gardens/ships/business/decorators/examples/multiple.py
--rw-r--r--   0        0        0        5 2023-08-24 19:13:50.976195 ships-1.2.8/fields/gardens/ships/cadence/UTC/UTC.r.HTML
--rw-r--r--   0        0        0      445 2023-08-24 18:30:42.487585 ships-1.2.8/fields/gardens/ships/cadence/UTC/__pycache__/MONTH_STRING.cpython-310.pyc
--rw-r--r--   0        0        0      473 2023-08-24 18:51:28.868547 ships-1.2.8/fields/gardens/ships/cadence/UTC/__pycache__/MONTH_STRINGS.cpython-310.pyc
--rw-r--r--   0        0        0      558 2023-09-20 23:22:24.125042 ships-1.2.8/fields/gardens/ships/cadence/UTC/__pycache__/MONTH_STRINGS.cpython-311.pyc
--rw-r--r--   0        0        0     1020 2023-08-24 19:16:27.758105 ships-1.2.8/fields/gardens/ships/cadence/UTC/__pycache__/NOW.cpython-310.pyc
--rw-r--r--   0        0        0     1501 2023-09-20 23:22:24.125042 ships-1.2.8/fields/gardens/ships/cadence/UTC/__pycache__/NOW.cpython-311.pyc
--rw-r--r--   0        0        0     1044 2024-02-15 04:18:41.492637 ships-1.2.8/fields/gardens/ships/cadence/UTC/__pycache__/current.cpython-310.pyc
--rw-r--r--   0        0        0     1359 2023-12-19 05:34:24.830799 ships-1.2.8/fields/gardens/ships/cadence/UTC/__pycache__/current.cpython-311.pyc
--rw-r--r--   0        0        0     1536 2023-11-10 20:12:48.854953 ships-1.2.8/fields/gardens/ships/cadence/UTC/__pycache__/now.cpython-311.pyc
--rw-r--r--   0        0        0      805 2024-04-17 00:30:27.148287 ships-1.2.8/fields/gardens/ships/cadence/UTC/__pycache__/status_current.cpython-310.pyc
--rw-r--r--   0        0        0     1864 2023-08-26 16:58:15.682142 ships-1.2.8/fields/gardens/ships/cadence/UTC/__pycache__/test_NOW.cpython-310-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     4602 2023-09-20 23:22:24.124042 ships-1.2.8/fields/gardens/ships/cadence/UTC/__pycache__/test_NOW.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0      958 2023-12-19 05:34:09.985917 ships-1.2.8/fields/gardens/ships/cadence/UTC/current.py
--rw-r--r--   0        0        0        0 2023-08-24 19:08:54.245033 ships-1.2.8/fields/gardens/ships/cadence/UTC/leap/seconds.py
--rw-r--r--   0        0        0        0 2023-08-24 19:08:50.249109 ships-1.2.8/fields/gardens/ships/cadence/UTC/leap/years.py
--rw-r--r--   0        0        0      626 2024-02-15 04:18:41.492637 ships-1.2.8/fields/gardens/ships/cadence/UTC/month/__pycache__/strings.cpython-310.pyc
--rw-r--r--   0        0        0      781 2023-12-19 05:34:24.831799 ships-1.2.8/fields/gardens/ships/cadence/UTC/month/__pycache__/strings.cpython-311.pyc
--rw-r--r--   0        0        0      440 2023-12-19 05:34:09.996917 ships-1.2.8/fields/gardens/ships/cadence/UTC/month/strings.py
--rw-r--r--   0        0        0      604 2023-12-19 05:34:10.009917 ships-1.2.8/fields/gardens/ships/cadence/UTC/status_current.py
--rw-r--r--   0        0        0     2005 2023-12-19 05:34:09.938917 ships-1.2.8/fields/gardens/ships/cadence/filter/__init__.py
--rw-r--r--   0        0        0     2687 2024-02-15 04:18:37.484684 ships-1.2.8/fields/gardens/ships/cadence/filter/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4059 2023-12-19 05:34:23.338811 ships-1.2.8/fields/gardens/ships/cadence/filter/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      843 2024-04-17 00:30:27.116287 ships-1.2.8/fields/gardens/ships/cadence/filter/_status/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0     1034 2024-04-17 00:30:26.956290 ships-1.2.8/fields/gardens/ships/cadence/filter/_status/__pycache__/status_2.cpython-310.pyc
--rw-r--r--   0        0        0     1077 2024-04-17 00:30:27.000289 ships-1.2.8/fields/gardens/ships/cadence/filter/_status/__pycache__/status_3.cpython-310.pyc
--rw-r--r--   0        0        0      533 2023-12-19 05:34:09.949917 ships-1.2.8/fields/gardens/ships/cadence/filter/_status/status_1.py
--rw-r--r--   0        0        0      873 2023-12-19 05:34:09.960917 ships-1.2.8/fields/gardens/ships/cadence/filter/_status/status_2.py
--rw-r--r--   0        0        0      961 2023-12-19 05:34:09.973917 ships-1.2.8/fields/gardens/ships/cadence/filter/_status/status_3.py
--rw-r--r--   0        0        0      279 2023-11-10 20:08:24.789837 ships-1.2.8/fields/gardens/ships/cadence/orbits/orbits.r.html
--rw-r--r--   0        0        0        2 2023-11-27 01:22:43.950708 ships-1.2.8/fields/gardens/ships/clique.py
--rw-r--r--   0        0        0      117 2023-12-01 16:30:53.383074 ships-1.2.8/fields/gardens/ships/coms/coms.r.HTML
--rw-r--r--   0        0        0      525 2023-12-01 14:37:22.097515 ships-1.2.8/fields/gardens/ships/coms/protocols/SSH/SSH.r.HTML
--rw-r--r--   0        0        0      186 2023-12-01 21:53:45.724017 ships-1.2.8/fields/gardens/ships/coms/protocols/SSL/SSL.r.HTML
--rw-r--r--   0        0        0        2 2023-12-01 16:29:57.831848 ships-1.2.8/fields/gardens/ships/coms/wall/wall.r.HTML
--rw-r--r--   0        0        0      184 2023-12-19 05:34:10.022917 ships-1.2.8/fields/gardens/ships/cycle/__init__.py
--rw-r--r--   0        0        0      420 2024-02-15 04:18:37.444684 ships-1.2.8/fields/gardens/ships/cycle/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      522 2023-12-19 05:34:23.357811 ships-1.2.8/fields/gardens/ships/cycle/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1850 2023-11-08 18:21:02.370631 ships-1.2.8/fields/gardens/ships/cycle/__pycache__/loops.cpython-311.pyc
--rw-r--r--   0        0        0      878 2023-11-08 18:22:42.926530 ships-1.2.8/fields/gardens/ships/cycle/__pycache__/params.cpython-311.pyc
--rw-r--r--   0        0        0      883 2023-11-08 18:27:36.336319 ships-1.2.8/fields/gardens/ships/cycle/__pycache__/presents.cpython-311.pyc
--rw-r--r--   0        0        0      610 2024-04-09 19:03:39.047772 ships-1.2.8/fields/gardens/ships/cycle/cycle.S.HTML
--rw-r--r--   0        0        0     1715 2024-04-09 18:50:19.806097 ships-1.2.8/fields/gardens/ships/cycle/loops/__init__.py
--rw-r--r--   0        0        0     1233 2024-04-16 02:27:49.074085 ships-1.2.8/fields/gardens/ships/cycle/loops/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2009 2024-01-06 04:04:08.042839 ships-1.2.8/fields/gardens/ships/cycle/loops/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      915 2024-04-17 00:30:27.124287 ships-1.2.8/fields/gardens/ships/cycle/loops/__pycache__/status_2.cpython-310.pyc
--rw-r--r--   0        0        0      906 2024-04-17 00:30:27.148287 ships-1.2.8/fields/gardens/ships/cycle/loops/__pycache__/status_3.cpython-310.pyc
--rw-r--r--   0        0        0      970 2024-04-17 00:30:27.004289 ships-1.2.8/fields/gardens/ships/cycle/loops/__pycache__/status_4.cpython-310.pyc
--rw-r--r--   0        0        0        6 2023-11-12 17:53:20.244810 ships-1.2.8/fields/gardens/ships/cycle/loops/loops.s.HTML
--rw-r--r--   0        0        0      711 2023-12-19 05:47:03.340798 ships-1.2.8/fields/gardens/ships/cycle/loops/status_2.py
--rw-r--r--   0        0        0      622 2023-12-19 05:34:10.055916 ships-1.2.8/fields/gardens/ships/cycle/loops/status_3.py
--rw-r--r--   0        0        0      716 2023-12-19 05:34:10.066916 ships-1.2.8/fields/gardens/ships/cycle/loops/status_4.py
--rw-r--r--   0        0        0      658 2023-11-12 18:07:23.961957 ships-1.2.8/fields/gardens/ships/cycle/params/__init__.py
--rw-r--r--   0        0        0      672 2024-02-15 04:18:37.476684 ships-1.2.8/fields/gardens/ships/cycle/params/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      968 2023-11-12 18:07:25.924936 ships-1.2.8/fields/gardens/ships/cycle/params/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      679 2024-04-17 00:30:26.880291 ships-1.2.8/fields/gardens/ships/cycle/params/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0      758 2024-04-17 00:30:27.096288 ships-1.2.8/fields/gardens/ships/cycle/params/__pycache__/status_2.cpython-310.pyc
--rw-r--r--   0        0        0      433 2023-12-19 05:34:10.077916 ships-1.2.8/fields/gardens/ships/cycle/params/status_1.py
--rw-r--r--   0        0        0      536 2023-12-19 05:34:10.088916 ships-1.2.8/fields/gardens/ships/cycle/params/status_2.py
--rw-r--r--   0        0        0      940 2024-01-06 04:12:45.342082 ships-1.2.8/fields/gardens/ships/cycle/params_2/__init__.py
--rw-r--r--   0        0        0      873 2024-02-15 04:18:40.316651 ships-1.2.8/fields/gardens/ships/cycle/params_2/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1289 2024-01-06 04:13:16.981731 ships-1.2.8/fields/gardens/ships/cycle/params_2/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1005 2024-04-17 00:30:27.088288 ships-1.2.8/fields/gardens/ships/cycle/params_2/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0      853 2023-12-28 20:22:31.165818 ships-1.2.8/fields/gardens/ships/cycle/params_2/status_1.py
--rw-r--r--   0        0        0      313 2023-12-19 05:34:10.129916 ships-1.2.8/fields/gardens/ships/cycle/presents/__init__.py
--rw-r--r--   0        0        0      671 2024-02-15 04:18:37.444684 ships-1.2.8/fields/gardens/ships/cycle/presents/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      893 2023-12-19 05:34:23.627809 ships-1.2.8/fields/gardens/ships/cycle/presents/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1175 2023-12-19 05:34:10.140916 ships-1.2.8/fields/gardens/ships/flow/demux_mux/__init__.py
--rw-r--r--   0        0        0     1555 2024-02-15 04:18:37.496683 ships-1.2.8/fields/gardens/ships/flow/demux_mux/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2435 2023-12-19 05:34:23.355811 ships-1.2.8/fields/gardens/ships/flow/demux_mux/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1448 2024-04-17 00:30:26.780292 ships-1.2.8/fields/gardens/ships/flow/demux_mux/_status/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0     1056 2023-12-19 05:34:10.152916 ships-1.2.8/fields/gardens/ships/flow/demux_mux/_status/status_1.py
--rw-r--r--   0        0        0      334 2023-11-27 01:18:22.607776 ships-1.2.8/fields/gardens/ships/flow/demux_mux/demux_mux.r.html
--rw-r--r--   0        0        0      830 2023-12-19 05:34:10.162916 ships-1.2.8/fields/gardens/ships/flow/demux_mux2/__init__.py
--rw-r--r--   0        0        0      830 2024-02-15 04:18:37.472684 ships-1.2.8/fields/gardens/ships/flow/demux_mux2/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1187 2023-12-19 05:34:23.355811 ships-1.2.8/fields/gardens/ships/flow/demux_mux2/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      805 2024-04-17 00:30:27.000289 ships-1.2.8/fields/gardens/ships/flow/demux_mux2/_status/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0      515 2023-12-19 05:34:10.174915 ships-1.2.8/fields/gardens/ships/flow/demux_mux2/_status/status_1.py
--rw-r--r--   0        0        0      285 2023-11-08 16:55:45.185683 ships-1.2.8/fields/gardens/ships/flow/flow.s.HTML
--rw-r--r--   0        0        0     1402 2024-03-17 03:19:08.657130 ships-1.2.8/fields/gardens/ships/flow/simultaneous/__init__.py
--rw-r--r--   0        0        0      919 2024-01-19 20:43:25.697218 ships-1.2.8/fields/gardens/ships/formats/ISO/ISO.s.HTML
--rw-r--r--   0        0        0     6927 2023-11-18 21:15:34.850274 ships-1.2.8/fields/gardens/ships/glamour/UTF8/one.HTML
--rw-r--r--   0        0        0      814 2024-02-15 04:18:37.464684 ships-1.2.8/fields/gardens/ships/insure/__pycache__/equalities.cpython-310.pyc
--rw-r--r--   0        0        0     1249 2023-12-19 05:34:23.625809 ships-1.2.8/fields/gardens/ships/insure/__pycache__/equalities.cpython-311.pyc
--rw-r--r--   0        0        0      694 2023-11-22 19:22:56.114817 ships-1.2.8/fields/gardens/ships/insure/__pycache__/equality.cpython-311.pyc
--rw-r--r--   0        0        0      555 2024-04-17 00:30:26.724293 ships-1.2.8/fields/gardens/ships/insure/__pycache__/status_equalitites_1.cpython-310.pyc
--rw-r--r--   0        0        0      690 2023-12-19 05:34:10.189915 ships-1.2.8/fields/gardens/ships/insure/equalities.py
--rw-r--r--   0        0        0      231 2023-12-19 05:34:10.201915 ships-1.2.8/fields/gardens/ships/insure/equality.py
--rw-r--r--   0        0        0      371 2023-12-19 05:34:10.213915 ships-1.2.8/fields/gardens/ships/insure/status_equalitites_1.py
--rw-r--r--   0        0        0     1108 2024-03-30 19:19:49.968672 ships-1.2.8/fields/gardens/ships/module.MD
--rw-r--r--   0        0        0      626 2024-03-17 02:48:33.516262 ships-1.2.8/fields/gardens/ships/modules/exceptions/__pycache__/parse.cpython-310.pyc
--rw-r--r--   0        0        0      884 2023-12-19 05:34:23.635809 ships-1.2.8/fields/gardens/ships/modules/exceptions/__pycache__/parse.cpython-311.pyc
--rw-r--r--   0        0        0      221 2023-11-29 22:52:11.709614 ships-1.2.8/fields/gardens/ships/modules/exceptions/custom/__init__.py
--rw-r--r--   0        0        0      445 2024-03-10 22:49:28.895330 ships-1.2.8/fields/gardens/ships/modules/exceptions/parse.py
--rw-r--r--   0        0        0      845 2023-12-19 05:34:10.235915 ships-1.2.8/fields/gardens/ships/modules/fasten/__init__.py
--rw-r--r--   0        0        0      858 2024-02-15 04:18:37.508683 ships-1.2.8/fields/gardens/ships/modules/fasten/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1330 2023-12-19 05:34:23.630809 ships-1.2.8/fields/gardens/ships/modules/fasten/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      351 2024-02-15 04:18:37.564683 ships-1.2.8/fields/gardens/ships/modules/fasten/_status/__pycache__/example.cpython-310.pyc
--rw-r--r--   0        0        0      415 2023-10-31 18:11:04.388642 ships-1.2.8/fields/gardens/ships/modules/fasten/_status/__pycache__/example.cpython-311.pyc
--rw-r--r--   0        0        0      447 2024-02-15 04:18:37.508683 ships-1.2.8/fields/gardens/ships/modules/fasten/_status/__pycache__/example_caller.cpython-310.pyc
--rw-r--r--   0        0        0      587 2023-12-19 05:34:23.632809 ships-1.2.8/fields/gardens/ships/modules/fasten/_status/__pycache__/example_caller.cpython-311.pyc
--rw-r--r--   0        0        0      522 2024-04-17 00:30:26.704293 ships-1.2.8/fields/gardens/ships/modules/fasten/_status/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0       46 2023-10-31 18:06:14.891051 ships-1.2.8/fields/gardens/ships/modules/fasten/_status/example.py
--rw-r--r--   0        0        0      121 2023-12-19 05:34:10.246915 ships-1.2.8/fields/gardens/ships/modules/fasten/_status/example_caller.py
--rw-r--r--   0        0        0      255 2023-12-19 05:34:10.257915 ships-1.2.8/fields/gardens/ships/modules/fasten/_status/status_1.py
--rw-r--r--   0        0        0      254 2023-11-28 04:58:18.174208 ships-1.2.8/fields/gardens/ships/modules/import/examples/__pycache__/example_1_module.cpython-311.pyc
--rw-r--r--   0        0        0      364 2023-11-28 05:02:32.938052 ships-1.2.8/fields/gardens/ships/modules/import/examples/example_1.py
--rw-r--r--   0        0        0        0 2023-11-28 04:57:58.030378 ships-1.2.8/fields/gardens/ships/modules/import/examples/example_1_module.py
--rw-r--r--   0        0        0      382 2023-11-30 01:01:28.804136 ships-1.2.8/fields/gardens/ships/modules/import/import.r.HTML
--rw-r--r--   0        0        0      679 2023-11-27 01:32:02.156155 ships-1.2.8/fields/gardens/ships/modules/print/print.s.HTML
--rw-r--r--   0        0        0       59 2023-12-17 22:23:07.000749 ships-1.2.8/fields/gardens/ships/modules/string/NLP/NLP.s.HTML
--rw-r--r--   0        0        0      265 2023-11-12 18:56:01.444149 ships-1.2.8/fields/gardens/ships/modules/string/end_of_string_is.py
--rw-r--r--   0        0        0       93 2023-12-17 22:25:39.567979 ships-1.2.8/fields/gardens/ships/modules/string/sayings/sayings.s.HTML
--rw-r--r--   0        0        0      223 2023-12-01 04:01:32.322888 ships-1.2.8/fields/gardens/ships/paths/caller.py
--rw-r--r--   0        0        0     3453 2024-02-15 05:14:15.432421 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/__init__.py
--rw-r--r--   0        0        0     2534 2024-02-15 05:15:22.147687 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3944 2023-12-19 05:34:23.327811 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      956 2024-04-17 00:30:26.768292 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/_status/1/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0        0 2023-09-26 17:01:19.501305 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/_status/1/directories/EQ_1/1.HTML
--rw-r--r--   0        0        0        0 2023-09-26 17:01:24.477254 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/_status/1/directories/EQ_2/1.HTML
--rw-r--r--   0        0        0      587 2024-02-15 05:03:56.927189 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/_status/1/status_1.py
--rw-r--r--   0        0        0     1018 2024-04-17 00:30:26.772292 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/_status/2/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0        0 2023-09-26 17:12:57.126345 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/_status/2/directories/EQ_1/1/1.HTML
--rw-r--r--   0        0        0        0 2023-09-26 17:12:39.434518 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/_status/2/directories/EQ_1/1.HTML
--rw-r--r--   0        0        0        0 2023-09-26 17:13:01.703300 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/_status/2/directories/EQ_2/1/2.HTML
--rw-r--r--   0        0        0        0 2023-09-26 17:12:42.709486 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/_status/2/directories/EQ_2/2.HTML
--rw-r--r--   0        0        0      682 2023-12-19 05:34:10.289914 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/_status/2/status_1.py
--rw-r--r--   0        0        0        3 2024-02-15 04:09:56.998834 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/clique.py
--rw-r--r--   0        0        0     1225 2023-09-26 17:25:34.940919 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/ADD_DIFFERENT_CONTENTS.cpython-311.pyc
--rw-r--r--   0        0        0     1082 2023-09-26 17:24:58.886273 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/ADD_DIFFERENT_PATHS.cpython-311.pyc
--rw-r--r--   0        0        0      767 2023-09-26 17:19:39.017407 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/GET_DIRECTORIES.cpython-311.pyc
--rw-r--r--   0        0        0      868 2023-09-26 17:20:39.552814 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/GET_SAME_DIRECTORIES.cpython-311.pyc
--rw-r--r--   0        0        0      435 2023-09-26 17:18:11.864261 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/IS_DIR.cpython-311.pyc
--rw-r--r--   0        0        0      822 2024-02-15 04:17:31.001458 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/add_different_contents.cpython-310.pyc
--rw-r--r--   0        0        0     1287 2023-12-03 23:12:22.567309 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/add_different_contents.cpython-311.pyc
--rw-r--r--   0        0        0      738 2024-02-15 04:17:31.001458 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/add_different_paths.cpython-310.pyc
--rw-r--r--   0        0        0     1115 2023-12-03 23:12:22.567309 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/add_different_paths.cpython-311.pyc
--rw-r--r--   0        0        0      589 2024-02-15 04:17:31.001458 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/get_directories.cpython-310.pyc
--rw-r--r--   0        0        0      800 2023-12-03 23:12:22.566310 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/get_directories.cpython-311.pyc
--rw-r--r--   0        0        0      650 2024-02-15 04:17:31.001458 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/get_same_directories.cpython-310.pyc
--rw-r--r--   0        0        0      901 2023-12-03 23:12:22.566310 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/get_same_directories.cpython-311.pyc
--rw-r--r--   0        0        0      393 2024-02-15 04:17:30.997458 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/is_dir.cpython-310.pyc
--rw-r--r--   0        0        0      469 2023-12-03 23:12:22.566310 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/is_dir.cpython-311.pyc
--rw-r--r--   0        0        0      702 2023-12-03 23:10:11.791819 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/add_different_contents.py
--rw-r--r--   0        0        0      575 2023-12-03 23:10:11.805819 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/add_different_paths.py
--rw-r--r--   0        0        0      291 2023-12-03 23:10:11.818818 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/get_directories.py
--rw-r--r--   0        0        0      431 2023-12-03 23:10:11.830819 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/get_same_directories.py
--rw-r--r--   0        0        0       70 2023-12-03 21:57:50.893795 ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/is_dir.py
--rw-r--r--   0        0        0      165 2023-12-19 05:34:10.300914 ships-1.2.8/fields/gardens/ships/paths/directory/deallocate/__init__.py
--rw-r--r--   0        0        0      494 2024-02-15 04:18:37.464684 ships-1.2.8/fields/gardens/ships/paths/directory/deallocate/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      585 2023-12-19 05:34:23.325811 ships-1.2.8/fields/gardens/ships/paths/directory/deallocate/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      142 2023-10-13 23:54:15.372867 ships-1.2.8/fields/gardens/ships/paths/directory/directory.html
--rw-r--r--   0        0        0     2162 2024-04-07 02:50:44.194867 ships-1.2.8/fields/gardens/ships/paths/directory/equalize/__init__.py
--rw-r--r--   0        0        0     2035 2024-04-07 02:50:55.966733 ships-1.2.8/fields/gardens/ships/paths/directory/equalize/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2556 2024-01-14 00:41:51.174597 ships-1.2.8/fields/gardens/ships/paths/directory/equalize/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1461 2024-04-17 00:30:26.756292 ships-1.2.8/fields/gardens/ships/paths/directory/equalize/_status/1/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0       10 2023-10-14 00:40:16.169744 ships-1.2.8/fields/gardens/ships/paths/directory/equalize/_status/1/start/1/1.py
--rw-r--r--   0        0        0        7 2023-10-14 00:57:00.845808 ships-1.2.8/fields/gardens/ships/paths/directory/equalize/_status/1/start/2/2.txt
--rw-r--r--   0        0        0        4 2023-10-14 00:56:55.910862 ships-1.2.8/fields/gardens/ships/paths/directory/equalize/_status/1/start/3/3.txt
--rw-r--r--   0        0        0     1387 2024-03-30 03:49:06.306137 ships-1.2.8/fields/gardens/ships/paths/directory/equalize/_status/1/status_1.py
--rw-r--r--   0        0        0     1392 2024-04-17 00:30:26.728293 ships-1.2.8/fields/gardens/ships/paths/directory/equalize/_status/2/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0       10 2023-10-14 00:40:16.169744 ships-1.2.8/fields/gardens/ships/paths/directory/equalize/_status/2/start/1/1.py
--rw-r--r--   0        0        0        7 2023-10-14 00:57:00.845808 ships-1.2.8/fields/gardens/ships/paths/directory/equalize/_status/2/start/2/2.txt
--rw-r--r--   0        0        0        0 2023-10-14 01:31:12.050509 ships-1.2.8/fields/gardens/ships/paths/directory/equalize/_status/2/start/2/55/55.txt
--rw-r--r--   0        0        0        4 2023-10-14 00:56:55.910862 ships-1.2.8/fields/gardens/ships/paths/directory/equalize/_status/2/start/3/3.txt
--rw-r--r--   0        0        0        0 2023-10-14 01:31:02.205616 ships-1.2.8/fields/gardens/ships/paths/directory/equalize/_status/2/start/3/9/9.txt
--rw-r--r--   0        0        0     1284 2023-12-19 05:34:10.344914 ships-1.2.8/fields/gardens/ships/paths/directory/equalize/_status/2/status_1.py
--rw-r--r--   0        0        0      101 2023-10-13 23:54:40.745591 ships-1.2.8/fields/gardens/ships/paths/directory/equalize/equalize.S.HTML
--rw-r--r--   0        0        0     1598 2024-04-12 21:58:19.908257 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/__init__.py
--rw-r--r--   0        0        0     1239 2024-04-16 02:27:49.606078 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2655 2023-12-19 05:34:23.624809 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1512 2024-04-17 00:30:26.804292 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/1.contents/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0        8 2023-11-09 18:10:08.040409 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/1.contents/cryo/1/example.html
--rw-r--r--   0        0        0     1113 2024-03-30 05:25:31.843636 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/1.contents/status_1.py
--rw-r--r--   0        0        0     1708 2024-04-17 00:30:27.056288 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/2.contents/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0        8 2023-11-09 18:10:08.040409 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/2.contents/cryo/1/example.html
--rw-r--r--   0        0        0       22 2024-03-30 04:06:34.621842 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/2.contents/cryo/S.HTML
--rw-r--r--   0        0        0       16 2024-03-30 04:06:46.557705 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/2.contents/cryo/another_place/place.HTML
--rw-r--r--   0        0        0     1349 2024-03-30 05:25:43.287496 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/2.contents/status_1.py
--rw-r--r--   0        0        0       10 2023-10-14 00:40:16.169744 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/3.contents_and_paths/temp/1/1.py
--rw-r--r--   0        0        0        0 2024-03-30 05:00:29.274092 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/3.contents_and_paths/temp/1.txt
--rw-r--r--   0        0        0        7 2023-10-14 00:57:00.845808 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/3.contents_and_paths/temp/2/2.txt
--rw-r--r--   0        0        0        0 2023-10-14 01:31:12.050509 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/3.contents_and_paths/temp/2/55/55.txt
--rw-r--r--   0        0        0        4 2023-10-14 00:56:55.910861 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/3.contents_and_paths/temp/3/3.txt
--rw-r--r--   0        0        0        0 2023-10-14 01:31:02.205616 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/3.contents_and_paths/temp/3/9/9.txt
--rw-r--r--   0        0        0       10 2023-10-14 00:40:16.169744 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/3.contents_and_paths/temp/symlink_to_1/1.py
--rw-r--r--   0        0        0        0 2024-03-30 05:00:29.274092 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/3.contents_and_paths/temp/symlink_to_1.txt
--rw-r--r--   0        0        0      196 2024-03-30 04:06:11.050111 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/field.S.HTML
--rw-r--r--   0        0        0      115 2023-10-21 23:43:14.421112 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/in_path.py
--rw-r--r--   0        0        0     3636 2024-04-16 02:26:41.806881 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/__init__.py
--rw-r--r--   0        0        0     2426 2024-04-16 02:27:49.110084 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2655 2023-12-19 05:34:23.624809 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1514 2024-04-17 00:30:27.056288 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/1.contents/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0        8 2023-11-09 18:10:08.040409 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/1.contents/cryo/example.html
--rw-r--r--   0        0        0     1117 2024-03-30 18:35:45.388509 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/1.contents/status_1.py
--rw-r--r--   0        0        0     1733 2024-04-17 00:30:26.924290 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/2.contents/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0        8 2023-11-09 18:10:08.040409 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/2.contents/cryo/1/example.html
--rw-r--r--   0        0        0       22 2024-03-30 04:06:34.621841 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/2.contents/cryo/S.HTML
--rw-r--r--   0        0        0       16 2024-03-30 04:06:46.557705 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/2.contents/cryo/another_place/place.HTML
--rw-r--r--   0        0        0     1358 2024-03-30 19:02:42.946268 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/2.contents/status_1.py
--rw-r--r--   0        0        0     2128 2024-04-17 00:30:27.112287 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0       10 2023-10-14 00:40:16.169744 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo/1/1.py
--rw-r--r--   0        0        0        0 2024-03-30 05:00:29.274092 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo/1.txt
--rw-r--r--   0        0        0        7 2023-10-14 00:57:00.845808 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo/2/2.txt
--rw-r--r--   0        0        0        0 2023-10-14 01:31:12.050509 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo/2/55/55.txt
--rw-r--r--   0        0        0        4 2023-10-14 00:56:55.910861 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo/3/3.txt
--rw-r--r--   0        0        0        0 2023-10-14 01:31:02.205616 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo/3/9/9.txt
--rw-r--r--   0        0        0       15 2024-03-30 18:35:01.213003 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo/txt/something.txt
--rw-r--r--   0        0        0       10 2023-10-14 00:40:16.169744 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo_proceeds/1/1.py
--rw-r--r--   0        0        0        0 2024-03-30 05:00:29.274092 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo_proceeds/1.the_txt
--rw-r--r--   0        0        0        7 2023-10-14 00:57:00.845808 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo_proceeds/2/2.the_txt
--rw-r--r--   0        0        0        0 2023-10-14 01:31:12.050509 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo_proceeds/2/55/55.the_txt
--rw-r--r--   0        0        0        4 2023-10-14 00:56:55.910861 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo_proceeds/3/3.the_txt
--rw-r--r--   0        0        0        0 2023-10-14 01:31:02.205616 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo_proceeds/3/9/9.the_txt
--rw-r--r--   0        0        0       10 2023-10-14 00:40:16.169744 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo_proceeds/symlink_to_1/1.py
--rw-r--r--   0        0        0        0 2024-03-30 05:00:29.274092 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo_proceeds/symlink_to_1.the_txt
--rw-r--r--   0        0        0       19 2024-03-30 18:54:24.571904 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo_proceeds/the_txt/something.the_txt
--rw-r--r--   0        0        0     1881 2024-03-30 18:59:07.456706 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/status_1.py
--rw-r--r--   0        0        0       10 2023-10-14 00:40:16.169744 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/temp/1/1.py
--rw-r--r--   0        0        0        0 2024-03-30 05:00:29.274092 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/temp/1.the_txt
--rw-r--r--   0        0        0        7 2023-10-14 00:57:00.845808 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/temp/2/2.the_txt
--rw-r--r--   0        0        0        0 2023-10-14 01:31:12.050509 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/temp/2/55/55.the_txt
--rw-r--r--   0        0        0        4 2023-10-14 00:56:55.910861 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/temp/3/3.the_txt
--rw-r--r--   0        0        0        0 2023-10-14 01:31:02.205616 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/temp/3/9/9.the_txt
--rw-r--r--   0        0        0       10 2023-10-14 00:40:16.169744 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/temp/symlink_to_1/1.py
--rw-r--r--   0        0        0        0 2024-03-30 05:00:29.274092 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/temp/symlink_to_1.the_txt
--rw-r--r--   0        0        0       19 2024-04-17 00:30:27.160287 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/temp/the_txt/something.the_txt
--rw-r--r--   0        0        0      196 2024-03-30 04:06:11.050111 ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/field.S.HTML
--rw-r--r--   0        0        0      781 2023-10-21 23:50:37.854518 ships-1.2.8/fields/gardens/ships/paths/directory/for_each_path/__init__.py
--rw-r--r--   0        0        0     1797 2023-12-19 05:34:10.383914 ships-1.2.8/fields/gardens/ships/paths/directory/rsync/__init__.py
--rw-r--r--   0        0        0     1768 2024-02-15 04:18:37.480684 ships-1.2.8/fields/gardens/ships/paths/directory/rsync/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2500 2023-12-19 05:34:23.330811 ships-1.2.8/fields/gardens/ships/paths/directory/rsync/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      974 2024-03-30 18:50:21.894647 ships-1.2.8/fields/gardens/ships/paths/directory/scan_tree/DFS.py
--rw-r--r--   0        0        0     2200 2024-03-30 18:22:06.590291 ships-1.2.8/fields/gardens/ships/paths/directory/scan_tree/__init__.py
--rw-r--r--   0        0        0     2032 2024-03-30 18:03:59.648399 ships-1.2.8/fields/gardens/ships/paths/directory/scan_tree/__init__v1.py
--rw-r--r--   0        0        0      676 2024-03-30 18:50:27.118588 ships-1.2.8/fields/gardens/ships/paths/directory/scan_tree/__pycache__/DFS.cpython-310.pyc
--rw-r--r--   0        0        0     1426 2024-03-30 18:22:08.390268 ships-1.2.8/fields/gardens/ships/paths/directory/scan_tree/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2076 2024-04-17 00:30:27.084288 ships-1.2.8/fields/gardens/ships/paths/directory/scan_tree/_status/1/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0       10 2023-10-14 00:40:16.169744 ships-1.2.8/fields/gardens/ships/paths/directory/scan_tree/_status/1/cryo/1/1.py
--rw-r--r--   0        0        0        0 2024-03-30 05:00:29.274092 ships-1.2.8/fields/gardens/ships/paths/directory/scan_tree/_status/1/cryo/1.txt
--rw-r--r--   0        0        0        7 2023-10-14 00:57:00.845808 ships-1.2.8/fields/gardens/ships/paths/directory/scan_tree/_status/1/cryo/2/2.txt
--rw-r--r--   0        0        0        0 2023-10-14 01:31:12.050509 ships-1.2.8/fields/gardens/ships/paths/directory/scan_tree/_status/1/cryo/2/55/55.txt
--rw-r--r--   0        0        0        4 2023-10-14 00:56:55.910861 ships-1.2.8/fields/gardens/ships/paths/directory/scan_tree/_status/1/cryo/3/3.txt
--rw-r--r--   0        0        0        0 2023-10-14 01:31:02.205616 ships-1.2.8/fields/gardens/ships/paths/directory/scan_tree/_status/1/cryo/3/9/9.txt
--rw-r--r--   0        0        0     3629 2024-03-30 19:04:59.464724 ships-1.2.8/fields/gardens/ships/paths/directory/scan_tree/_status/1/status_1.py
--rw-r--r--   0        0        0     1343 2024-04-17 00:30:26.712293 ships-1.2.8/fields/gardens/ships/paths/directory/scan_tree/_status/2/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-03-30 17:46:36.128181 ships-1.2.8/fields/gardens/ships/paths/directory/scan_tree/_status/2/cryo.txt
--rw-r--r--   0        0        0     1020 2024-03-30 19:04:22.217145 ships-1.2.8/fields/gardens/ships/paths/directory/scan_tree/_status/2/status_1.py
--rw-r--r--   0        0        0     1212 2023-12-19 05:34:10.397914 ships-1.2.8/fields/gardens/ships/paths/directory/sense/__init__.py
--rw-r--r--   0        0        0     1768 2024-02-15 04:18:37.444684 ships-1.2.8/fields/gardens/ships/paths/directory/sense/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2584 2023-12-19 05:34:23.331811 ships-1.2.8/fields/gardens/ships/paths/directory/sense/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1021 2024-04-17 00:30:26.844291 ships-1.2.8/fields/gardens/ships/paths/directory/sense/_status/1/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0      826 2024-03-30 05:18:51.408533 ships-1.2.8/fields/gardens/ships/paths/directory/sense/_status/1/status_1.py
--rw-r--r--   0        0        0      763 2023-12-19 05:34:10.423913 ships-1.2.8/fields/gardens/ships/paths/directory/size/__init__.py
--rw-r--r--   0        0        0     1116 2024-02-15 04:18:37.476684 ships-1.2.8/fields/gardens/ships/paths/directory/size/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1819 2023-12-19 05:34:23.329811 ships-1.2.8/fields/gardens/ships/paths/directory/size/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      947 2024-04-17 00:30:26.992289 ships-1.2.8/fields/gardens/ships/paths/directory/size/_status/1/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0       34 2023-12-03 23:22:28.062362 ships-1.2.8/fields/gardens/ships/paths/directory/size/_status/1/cryo/hyper.HTML
--rw-r--r--   0        0        0      623 2023-12-19 05:34:10.435913 ships-1.2.8/fields/gardens/ships/paths/directory/size/_status/1/status_1.py
--rw-r--r--   0        0        0      544 2023-12-19 05:34:10.447913 ships-1.2.8/fields/gardens/ships/paths/files/scan/JSON/__init__.py
--rw-r--r--   0        0        0     1362 2023-11-09 20:55:25.502570 ships-1.2.8/fields/gardens/ships/paths/files/scan/JSON/__pycache__/JSON.cpython-311.pyc
--rw-r--r--   0        0        0      928 2024-02-15 04:18:37.480684 ships-1.2.8/fields/gardens/ships/paths/files/scan/JSON/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1378 2023-12-19 05:34:23.647809 ships-1.2.8/fields/gardens/ships/paths/files/scan/JSON/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0       15 2023-11-09 20:50:52.710653 ships-1.2.8/fields/gardens/ships/paths/files/scan/JSON/cryo/example.JSON
--rw-r--r--   0        0        0      868 2024-04-17 00:30:26.760292 ships-1.2.8/fields/gardens/ships/paths/files/scan/JSON/status/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0      534 2023-12-19 05:34:10.459913 ships-1.2.8/fields/gardens/ships/paths/files/scan/JSON/status/status_1.py
--rw-r--r--   0        0        0      932 2023-10-13 23:36:51.568242 ships-1.2.8/fields/gardens/ships/paths/fs, rsync details.r.html
--rw-r--r--   0        0        0      367 2023-10-13 23:35:46.146955 ships-1.2.8/fields/gardens/ships/paths/fs.r.html
--rw-r--r--   0        0        0      934 2023-11-09 20:55:40.948395 ships-1.2.8/fields/gardens/ships/paths/path/__pycache__/relative.cpython-311.pyc
--rw-r--r--   0        0        0      327 2023-12-19 05:34:10.470913 ships-1.2.8/fields/gardens/ships/paths/path/relative.py
--rw-r--r--   0        0        0      396 2024-03-30 18:12:33.670409 ships-1.2.8/fields/gardens/ships/paths/variety/__init__.py
--rw-r--r--   0        0        0      485 2024-03-30 18:15:40.351557 ships-1.2.8/fields/gardens/ships/paths/variety/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    12177 2024-01-23 00:01:37.980550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/ANSI.py
--rw-r--r--   0        0        0    13419 2024-01-23 00:01:37.980550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/FSM.py
--rw-r--r--   0        0        0     4089 2024-01-23 00:01:37.980550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__init__.py
--rw-r--r--   0        0        0    19876 2024-01-23 00:01:37.984550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/ANSI.cpython-311.pyc
--rw-r--r--   0        0        0    16297 2024-01-23 00:01:37.985550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/FSM.cpython-311.pyc
--rw-r--r--   0        0        0     4220 2024-02-15 04:18:39.816656 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4382 2024-01-23 00:01:37.985550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1043 2024-01-23 00:01:37.985550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/_async.cpython-311.pyc
--rw-r--r--   0        0        0     6850 2024-01-23 00:01:37.986550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/_async_pre_await.cpython-311.pyc
--rw-r--r--   0        0        0     6975 2024-01-23 00:01:37.986550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/_async_w_await.cpython-311.pyc
--rw-r--r--   0        0        0     1932 2024-02-15 04:18:39.820656 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0        0        0     2671 2024-01-23 00:01:37.987550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/exceptions.cpython-311.pyc
--rw-r--r--   0        0        0     9145 2024-02-15 04:18:39.832656 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/expect.cpython-310.pyc
--rw-r--r--   0        0        0    16905 2024-01-23 00:01:37.988550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/expect.cpython-311.pyc
--rw-r--r--   0        0        0     7983 2024-01-23 00:01:37.989550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/fdpexpect.cpython-311.pyc
--rw-r--r--   0        0        0     8932 2024-01-23 00:01:37.989550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/popen_spawn.cpython-311.pyc
--rw-r--r--   0        0        0    32161 2024-02-15 04:18:39.852656 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/pty_spawn.cpython-310.pyc
--rw-r--r--   0        0        0    44581 2024-01-23 00:01:37.992550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/pty_spawn.cpython-311.pyc
--rw-r--r--   0        0        0    23360 2024-01-23 00:01:37.993550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/pxssh.cpython-311.pyc
--rw-r--r--   0        0        0     7584 2024-01-23 00:01:37.994550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/replwrap.cpython-311.pyc
--rw-r--r--   0        0        0     5856 2024-02-15 04:18:39.860656 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/run.cpython-310.pyc
--rw-r--r--   0        0        0     7805 2024-01-23 00:01:37.994550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/run.cpython-311.pyc
--rw-r--r--   0        0        0    21594 2024-01-23 00:01:37.996550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/screen.cpython-311.pyc
--rw-r--r--   0        0        0     7302 2024-01-23 00:01:37.996550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/socket_pexpect.cpython-311.pyc
--rw-r--r--   0        0        0    17837 2024-02-15 04:18:39.856656 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/spawnbase.cpython-310.pyc
--rw-r--r--   0        0        0    25269 2024-01-23 00:01:37.998550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/spawnbase.cpython-311.pyc
--rw-r--r--   0        0        0     3850 2024-02-15 04:18:39.824657 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0     6357 2024-01-23 00:01:37.999550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0      907 2024-01-23 00:01:37.980550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/_async.py
--rw-r--r--   0        0        0     3465 2024-01-23 00:01:37.980550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/_async_pre_await.py
--rw-r--r--   0        0        0     3802 2024-01-23 00:01:37.980550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/_async_w_await.py
--rw-r--r--   0        0        0      419 2024-01-23 00:01:37.980550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/bashrc.sh
--rw-r--r--   0        0        0     1068 2024-01-23 00:01:37.980550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/exceptions.py
--rw-r--r--   0        0        0    13827 2024-01-23 00:01:37.981550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/expect.py
--rw-r--r--   0        0        0     5991 2024-01-23 00:01:37.981550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/fdpexpect.py
--rw-r--r--   0        0        0        4 2024-01-23 00:01:37.999550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/pexpect-4.9.0.dist-info/INSTALLER
--rw-r--r--   0        0        0      987 2024-01-23 00:01:37.982550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/pexpect-4.9.0.dist-info/LICENSE
--rw-r--r--   0        0        0     2463 2024-01-23 00:01:37.982550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/pexpect-4.9.0.dist-info/METADATA
--rw-r--r--   0        0        0     2900 2024-01-23 00:01:38.000550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/pexpect-4.9.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2024-01-23 00:01:37.999550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/pexpect-4.9.0.dist-info/REQUESTED
--rw-r--r--   0        0        0      110 2024-01-23 00:01:37.982550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/pexpect-4.9.0.dist-info/WHEEL
--rw-r--r--   0        0        0        8 2024-01-23 00:01:37.982550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/pexpect-4.9.0.dist-info/top_level.txt
--rw-r--r--   0        0        0     6159 2024-01-23 00:01:37.981550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/popen_spawn.py
--rw-r--r--   0        0        0    37382 2024-01-23 00:01:37.981550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/pty_spawn.py
--rw-r--r--   0        0        0    24445 2024-01-23 00:01:37.981550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/pxssh.py
--rw-r--r--   0        0        0     5951 2024-01-23 00:01:37.981550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/replwrap.py
--rw-r--r--   0        0        0     6629 2024-01-23 00:01:37.981550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/run.py
--rw-r--r--   0        0        0    13704 2024-01-23 00:01:37.982550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/screen.py
--rw-r--r--   0        0        0     4814 2024-01-23 00:01:37.982550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/socket_pexpect.py
--rw-r--r--   0        0        0    21685 2024-01-23 00:01:37.982550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/spawnbase.py
--rw-r--r--   0        0        0     6019 2024-01-23 00:01:37.982550 ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/utils.py
--rw-r--r--   0        0        0     1046 2024-02-15 04:18:41.940632 ships-1.2.8/fields/gardens/ships/ports/__pycache__/available.cpython-310.pyc
--rw-r--r--   0        0        0     1616 2023-12-19 05:34:24.854799 ships-1.2.8/fields/gardens/ships/ports/__pycache__/available.cpython-311.pyc
--rw-r--r--   0        0        0      638 2024-02-15 04:18:41.940632 ships-1.2.8/fields/gardens/ships/ports/__pycache__/claimed.cpython-310.pyc
--rw-r--r--   0        0        0      938 2023-12-19 05:34:24.854799 ships-1.2.8/fields/gardens/ships/ports/__pycache__/claimed.cpython-311.pyc
--rw-r--r--   0        0        0      606 2024-04-17 00:30:27.060288 ships-1.2.8/fields/gardens/ships/ports/_status/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0      507 2023-12-19 05:34:10.482913 ships-1.2.8/fields/gardens/ships/ports/_status/status_1.py
--rw-r--r--   0        0        0      983 2023-12-19 05:34:10.496913 ships-1.2.8/fields/gardens/ships/ports/available.py
--rw-r--r--   0        0        0      498 2023-12-19 05:34:10.507913 ships-1.2.8/fields/gardens/ships/ports/claimed.py
--rw-r--r--   0        0        0      631 2023-12-19 05:34:10.519913 ships-1.2.8/fields/gardens/ships/ports/find_multiple/__init__.py
--rw-r--r--   0        0        0      856 2024-02-15 04:18:41.936632 ships-1.2.8/fields/gardens/ships/ports/find_multiple/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1308 2023-12-19 05:34:24.854799 ships-1.2.8/fields/gardens/ships/ports/find_multiple/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      666 2024-04-17 00:30:27.080288 ships-1.2.8/fields/gardens/ships/ports/find_multiple/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0      419 2023-12-19 05:34:10.531913 ships-1.2.8/fields/gardens/ships/ports/find_multiple/status_1.py
--rw-r--r--   0        0        0     1756 2024-01-23 00:49:41.930690 ships-1.2.8/fields/gardens/ships/process/multi/__init__.py
--rw-r--r--   0        0        0     2030 2024-02-15 04:18:40.024654 ships-1.2.8/fields/gardens/ships/process/multi/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3162 2024-01-23 00:49:44.726658 ships-1.2.8/fields/gardens/ships/process/multi/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      891 2024-04-17 00:30:27.212286 ships-1.2.8/fields/gardens/ships/process/multi/_status/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0     1034 2024-04-17 00:30:27.240285 ships-1.2.8/fields/gardens/ships/process/multi/_status/__pycache__/status_2.cpython-310.pyc
--rw-r--r--   0        0        0      851 2023-12-19 05:34:10.553912 ships-1.2.8/fields/gardens/ships/process/multi/_status/status_1.py
--rw-r--r--   0        0        0      923 2024-01-23 03:58:21.718356 ships-1.2.8/fields/gardens/ships/process/multi/_status/status_2.py
--rw-r--r--   0        0        0     3733 2024-01-23 04:02:43.996412 ships-1.2.8/fields/gardens/ships/process/multi_2/__init__.py
--rw-r--r--   0        0        0     2725 2024-02-15 04:18:39.972655 ships-1.2.8/fields/gardens/ships/process/multi_2/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4843 2024-01-23 04:02:57.086266 ships-1.2.8/fields/gardens/ships/process/multi_2/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1536 2024-04-17 00:30:27.036288 ships-1.2.8/fields/gardens/ships/process/multi_2/_status/2/__pycache__/status_2.cpython-310.pyc
--rw-r--r--   0        0        0      180 2024-01-22 23:55:08.820853 ships-1.2.8/fields/gardens/ships/process/multi_2/_status/2/script.py
--rw-r--r--   0        0        0     1429 2024-01-23 04:15:28.615832 ships-1.2.8/fields/gardens/ships/process/multi_2/_status/2/status_2.py
--rw-r--r--   0        0        0     1241 2024-04-17 00:30:26.936290 ships-1.2.8/fields/gardens/ships/process/multi_2/_status/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0     1005 2024-01-23 03:59:33.397551 ships-1.2.8/fields/gardens/ships/process/multi_2/_status/status_1.py
--rw-r--r--   0        0        0     1605 2024-01-23 04:06:55.382592 ships-1.2.8/fields/gardens/ships/process/start/__init__.py
--rw-r--r--   0        0        0     1395 2024-02-15 04:18:39.816656 ships-1.2.8/fields/gardens/ships/process/start/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2026 2024-01-23 04:07:13.569387 ships-1.2.8/fields/gardens/ships/process/start/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    69632 2024-01-23 03:07:00.507890 ships-1.2.8/fields/gardens/ships/process/start/_status/.coverage
--rw-r--r--   0        0        0    69632 2024-01-23 04:02:47.177377 ships-1.2.8/fields/gardens/ships/process/start/_status/.status_1_coverage
--rw-r--r--   0        0        0    53248 2024-01-23 01:43:21.048331 ships-1.2.8/fields/gardens/ships/process/start/_status/2/.coverage
--rw-r--r--   0        0        0     1568 2024-04-17 00:30:26.896290 ships-1.2.8/fields/gardens/ships/process/start/_status/2/__pycache__/status_2.cpython-310.pyc
--rw-r--r--   0        0        0      160 2024-01-23 01:46:12.526385 ships-1.2.8/fields/gardens/ships/process/start/_status/2/script.py
--rw-r--r--   0        0        0     1495 2024-01-23 04:15:44.186657 ships-1.2.8/fields/gardens/ships/process/start/_status/2/status_2.py
--rw-r--r--   0        0        0     1546 2024-04-17 00:30:27.016289 ships-1.2.8/fields/gardens/ships/process/start/_status/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0     1169 2024-01-23 04:07:00.762531 ships-1.2.8/fields/gardens/ships/process/start/_status/status_1.py
--rw-r--r--   0        0        0      828 2024-02-15 04:18:40.124653 ships-1.2.8/fields/gardens/ships/process/start/parts/__pycache__/awareness.cpython-310.pyc
--rw-r--r--   0        0        0     1623 2024-01-23 03:06:26.360273 ships-1.2.8/fields/gardens/ships/process/start/parts/__pycache__/awareness.cpython-311.pyc
--rw-r--r--   0        0        0      647 2024-02-15 04:18:40.124653 ships-1.2.8/fields/gardens/ships/process/start/parts/__pycache__/returns.cpython-310.pyc
--rw-r--r--   0        0        0      842 2024-01-23 04:07:13.655386 ships-1.2.8/fields/gardens/ships/process/start/parts/__pycache__/returns.cpython-311.pyc
--rw-r--r--   0        0        0      916 2024-01-23 03:03:06.613515 ships-1.2.8/fields/gardens/ships/process/start/parts/awareness.py
--rw-r--r--   0        0        0      486 2024-01-23 04:06:27.768901 ships-1.2.8/fields/gardens/ships/process/start/parts/returns.py
--rw-r--r--   0        0        0       69 2023-12-19 05:34:10.556912 ships-1.2.8/fields/gardens/ships/revenue.py
--rw-r--r--   0        0        0        8 2023-12-19 05:32:53.977518 ships-1.2.8/fields/gardens/ships/ships.s.HTML
--rw-r--r--   0        0        0      584 2024-04-17 00:30:46.188025 ships-1.2.8/pyproject.toml
--rw-r--r--   0        0        0     1108 2024-03-30 19:19:57.188600 ships-1.2.8/readme.md
--rw-r--r--   0        0        0      884 2024-04-17 00:31:00.159834 ships-1.2.8/ships.S.HTML
--rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 ships-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0      104 2024-03-30 17:23:39.109806 ships-1.3.8/fields/gardens/ships/AMLI/AMLI.S.HTML
+-rw-r--r--   0        0        0       61 2024-02-15 19:38:33.618784 ships-1.3.8/fields/gardens/ships/AMLI/LLM/LLM.S.HTML
+-rw-r--r--   0        0        0       44 2024-02-15 19:38:43.658669 ships-1.3.8/fields/gardens/ships/Search/Search.s.HTML
+-rw-r--r--   0        0        0     1008 2024-02-15 04:11:24.069788 ships-1.3.8/fields/gardens/ships/__init__.py
+-rw-r--r--   0        0        0      547 2024-02-15 04:21:26.722722 ships-1.3.8/fields/gardens/ships/_clique/__init__.py
+-rw-r--r--   0        0        0     1004 2024-02-15 04:21:33.042649 ships-1.3.8/fields/gardens/ships/_clique/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      173 2023-12-16 19:52:14.770884 ships-1.3.8/fields/gardens/ships/_license/license.s.HTML
+-rw-r--r--   0        0        0    37279 2023-12-01 20:51:04.310266 ships-1.3.8/fields/gardens/ships/_license/licenses/gpl-3.0-standalone.html
+-rw-r--r--   0        0        0    69632 2024-01-23 00:08:48.421730 ships-1.3.8/fields/gardens/ships/_status/.coverage
+-rw-r--r--   0        0        0  1178208 2024-04-24 04:23:13.463172 ships-1.3.8/fields/gardens/ships/_status/DB/records.json
+-rw-r--r--   0        0        0       27 2024-01-23 00:04:12.188823 ships-1.3.8/fields/gardens/ships/_status/coverage_report/.gitignore
+-rw-r--r--   0        0        0    21865 2024-01-23 00:08:28.865949 ships-1.3.8/fields/gardens/ships/_status/coverage_report/coverage_html.js
+-rw-r--r--   0        0        0    49384 2024-01-23 00:08:28.743950 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_45774dabac2a4451___init___py.html
+-rw-r--r--   0        0        0    48035 2024-01-23 00:04:11.398832 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad___init___py.html
+-rw-r--r--   0        0        0   160908 2024-01-23 00:04:11.422832 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__cell_widths_py.html
+-rw-r--r--   0        0        0  1010994 2024-01-23 00:04:11.580830 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__emoji_codes_py.html
+-rw-r--r--   0        0        0    14114 2024-01-23 00:04:11.586830 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__emoji_replace_py.html
+-rw-r--r--   0        0        0    18535 2024-01-23 00:04:11.588830 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__export_format_py.html
+-rw-r--r--   0        0        0    10425 2024-01-23 00:04:11.589830 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__fileno_py.html
+-rw-r--r--   0        0        0    33320 2024-01-23 00:04:11.594830 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__log_render_py.html
+-rw-r--r--   0        0        0    16305 2024-01-23 00:04:11.597830 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__loop_py.html
+-rw-r--r--   0        0        0    22576 2024-01-23 00:04:11.600830 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__null_file_py.html
+-rw-r--r--   0        0        0   108791 2024-01-23 00:04:11.616830 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__palettes_py.html
+-rw-r--r--   0        0        0     8412 2024-01-23 00:04:11.618830 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__pick_py.html
+-rw-r--r--   0        0        0    48386 2024-01-23 00:04:11.625830 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__ratio_py.html
+-rw-r--r--   0        0        0    29373 2024-01-23 00:04:11.629830 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__wrap_py.html
+-rw-r--r--   0        0        0    12484 2024-01-23 00:04:11.631830 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_abc_py.html
+-rw-r--r--   0        0        0    91280 2024-01-23 00:04:11.655829 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_align_py.html
+-rw-r--r--   0        0        0   112963 2024-01-23 00:04:11.669829 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_box_py.html
+-rw-r--r--   0        0        0    47077 2024-01-23 00:04:11.677829 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_cells_py.html
+-rw-r--r--   0        0        0   176081 2024-01-23 00:04:11.702829 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_color_py.html
+-rw-r--r--   0        0        0    13311 2024-01-23 00:04:11.705829 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_color_triplet_py.html
+-rw-r--r--   0        0        0   717904 2024-01-23 00:04:11.818827 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_console_py.html
+-rw-r--r--   0        0        0    15230 2024-01-23 00:04:11.823828 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_constrain_py.html
+-rw-r--r--   0        0        0    54307 2024-01-23 00:04:11.832827 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_containers_py.html
+-rw-r--r--   0        0        0    62602 2024-01-23 00:04:11.841827 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_control_py.html
+-rw-r--r--   0        0        0    80963 2024-01-23 00:04:11.853827 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_default_styles_py.html
+-rw-r--r--   0        0        0    28704 2024-01-23 00:04:11.858827 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_emoji_py.html
+-rw-r--r--   0        0        0    11215 2024-01-23 00:04:11.859827 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_errors_py.html
+-rw-r--r--   0        0        0    60921 2024-01-23 00:04:11.866827 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_highlighter_py.html
+-rw-r--r--   0        0        0    41115 2024-01-23 00:04:11.872827 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_json_py.html
+-rw-r--r--   0        0        0    34765 2024-01-23 00:04:11.877827 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_jupyter_py.html
+-rw-r--r--   0        0        0    72977 2024-01-23 00:04:11.888827 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_markup_py.html
+-rw-r--r--   0        0        0    43367 2024-01-23 00:04:11.894827 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_measure_py.html
+-rw-r--r--   0        0        0    46862 2024-01-23 00:04:11.901827 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_padding_py.html
+-rw-r--r--   0        0        0    12954 2024-01-23 00:04:11.903827 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_pager_py.html
+-rw-r--r--   0        0        0    35002 2024-01-23 00:04:11.908826 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_palette_py.html
+-rw-r--r--   0        0        0    92571 2024-01-23 00:04:11.921826 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_panel_py.html
+-rw-r--r--   0        0        0   279872 2024-01-23 00:04:11.960826 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_pretty_py.html
+-rw-r--r--   0        0        0    15360 2024-01-23 00:04:11.963826 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_protocol_py.html
+-rw-r--r--   0        0        0     6679 2024-01-23 00:04:11.964826 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_region_py.html
+-rw-r--r--   0        0        0    47741 2024-01-23 00:04:11.972826 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_repr_py.html
+-rw-r--r--   0        0        0    28545 2024-01-23 00:04:11.976826 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_scope_py.html
+-rw-r--r--   0        0        0    18971 2024-01-23 00:04:11.978826 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_screen_py.html
+-rw-r--r--   0        0        0   197532 2024-01-23 00:04:12.016825 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_segment_py.html
+-rw-r--r--   0        0        0   232858 2024-01-23 00:04:12.050825 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_style_py.html
+-rw-r--r--   0        0        0    15742 2024-01-23 00:04:12.053825 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_styled_py.html
+-rw-r--r--   0        0        0   291082 2024-01-23 00:04:12.093824 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_table_py.html
+-rw-r--r--   0        0        0    49301 2024-01-23 00:04:12.101824 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_terminal_theme_py.html
+-rw-r--r--   0        0        0   384696 2024-01-23 00:04:12.168824 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_text_py.html
+-rw-r--r--   0        0        0    36139 2024-01-23 00:04:12.183823 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_theme_py.html
+-rw-r--r--   0        0        0     5766 2024-01-23 00:04:12.185824 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_themes_py.html
+-rw-r--r--   0        0        0    13616 2024-01-23 00:04:11.284834 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_9c84d462c231d294_exceptions_py.html
+-rw-r--r--   0        0        0   113380 2024-01-23 00:04:11.299833 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_9c84d462c231d294_expect_py.html
+-rw-r--r--   0        0        0   227312 2024-01-23 00:08:28.770950 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_9c84d462c231d294_pty_spawn_py.html
+-rw-r--r--   0        0        0   144953 2024-01-23 00:08:28.799950 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_9c84d462c231d294_spawnbase_py.html
+-rw-r--r--   0        0        0    52548 2024-01-23 00:04:11.363833 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_9c84d462c231d294_utils_py.html
+-rw-r--r--   0        0        0   228779 2024-01-23 00:08:28.829949 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_acd758f7e5b0fd78_ptyprocess_py.html
+-rw-r--r--   0        0        0    48168 2024-01-23 00:05:49.589733 ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_f85661004356945c___init___py.html
+-rw-r--r--   0        0        0     1732 2024-01-23 00:08:28.865949 ships-1.3.8/fields/gardens/ships/_status/coverage_report/favicon_32.png
+-rw-r--r--   0        0        0    26478 2024-01-23 00:08:28.864949 ships-1.3.8/fields/gardens/ships/_status/coverage_report/index.html
+-rw-r--r--   0        0        0     9004 2024-01-23 00:08:28.865949 ships-1.3.8/fields/gardens/ships/_status/coverage_report/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2024-01-23 00:08:28.865949 ships-1.3.8/fields/gardens/ships/_status/coverage_report/keybd_open.png
+-rw-r--r--   0        0        0    17880 2024-01-23 00:08:28.865949 ships-1.3.8/fields/gardens/ships/_status/coverage_report/status.json
+-rw-r--r--   0        0        0    12406 2024-01-23 00:08:28.865949 ships-1.3.8/fields/gardens/ships/_status/coverage_report/style.css
+-rw-r--r--   0        0        0      198 2024-01-23 03:57:34.614884 ships-1.3.8/fields/gardens/ships/_status/ports.py
+-rw-r--r--   0        0        0      994 2024-04-17 00:26:54.579284 ships-1.3.8/fields/gardens/ships/_status/status.proc.py
+-rw-r--r--   0        0        0       77 2023-11-22 19:02:46.200327 ships-1.3.8/fields/gardens/ships/business/business.s.HTML
+-rw-r--r--   0        0        0       65 2023-11-22 19:10:51.771905 ships-1.3.8/fields/gardens/ships/business/decorators/decorators.r.HTML
+-rw-r--r--   0        0        0      747 2023-11-22 19:15:14.376973 ships-1.3.8/fields/gardens/ships/business/decorators/examples/example_1.py
+-rw-r--r--   0        0        0       93 2023-11-22 19:09:40.879696 ships-1.3.8/fields/gardens/ships/business/decorators/examples/multiple.py
+-rw-r--r--   0        0        0        5 2023-08-24 19:13:50.976195 ships-1.3.8/fields/gardens/ships/cadence/UTC/UTC.r.HTML
+-rw-r--r--   0        0        0      445 2023-08-24 18:30:42.487585 ships-1.3.8/fields/gardens/ships/cadence/UTC/__pycache__/MONTH_STRING.cpython-310.pyc
+-rw-r--r--   0        0        0      473 2023-08-24 18:51:28.868547 ships-1.3.8/fields/gardens/ships/cadence/UTC/__pycache__/MONTH_STRINGS.cpython-310.pyc
+-rw-r--r--   0        0        0      558 2023-09-20 23:22:24.125042 ships-1.3.8/fields/gardens/ships/cadence/UTC/__pycache__/MONTH_STRINGS.cpython-311.pyc
+-rw-r--r--   0        0        0     1020 2023-08-24 19:16:27.758105 ships-1.3.8/fields/gardens/ships/cadence/UTC/__pycache__/NOW.cpython-310.pyc
+-rw-r--r--   0        0        0     1501 2023-09-20 23:22:24.125042 ships-1.3.8/fields/gardens/ships/cadence/UTC/__pycache__/NOW.cpython-311.pyc
+-rw-r--r--   0        0        0     1044 2024-02-15 04:18:41.492637 ships-1.3.8/fields/gardens/ships/cadence/UTC/__pycache__/current.cpython-310.pyc
+-rw-r--r--   0        0        0     1359 2023-12-19 05:34:24.830799 ships-1.3.8/fields/gardens/ships/cadence/UTC/__pycache__/current.cpython-311.pyc
+-rw-r--r--   0        0        0     1536 2023-11-10 20:12:48.854953 ships-1.3.8/fields/gardens/ships/cadence/UTC/__pycache__/now.cpython-311.pyc
+-rw-r--r--   0        0        0      805 2024-04-17 00:30:27.148287 ships-1.3.8/fields/gardens/ships/cadence/UTC/__pycache__/status_current.cpython-310.pyc
+-rw-r--r--   0        0        0     1864 2023-08-26 16:58:15.682142 ships-1.3.8/fields/gardens/ships/cadence/UTC/__pycache__/test_NOW.cpython-310-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     4602 2023-09-20 23:22:24.124042 ships-1.3.8/fields/gardens/ships/cadence/UTC/__pycache__/test_NOW.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0      958 2023-12-19 05:34:09.985917 ships-1.3.8/fields/gardens/ships/cadence/UTC/current.py
+-rw-r--r--   0        0        0        0 2023-08-24 19:08:54.245033 ships-1.3.8/fields/gardens/ships/cadence/UTC/leap/seconds.py
+-rw-r--r--   0        0        0        0 2023-08-24 19:08:50.249109 ships-1.3.8/fields/gardens/ships/cadence/UTC/leap/years.py
+-rw-r--r--   0        0        0      626 2024-02-15 04:18:41.492637 ships-1.3.8/fields/gardens/ships/cadence/UTC/month/__pycache__/strings.cpython-310.pyc
+-rw-r--r--   0        0        0      781 2023-12-19 05:34:24.831799 ships-1.3.8/fields/gardens/ships/cadence/UTC/month/__pycache__/strings.cpython-311.pyc
+-rw-r--r--   0        0        0      440 2023-12-19 05:34:09.996917 ships-1.3.8/fields/gardens/ships/cadence/UTC/month/strings.py
+-rw-r--r--   0        0        0      604 2023-12-19 05:34:10.009917 ships-1.3.8/fields/gardens/ships/cadence/UTC/status_current.py
+-rw-r--r--   0        0        0     2005 2023-12-19 05:34:09.938917 ships-1.3.8/fields/gardens/ships/cadence/filter/__init__.py
+-rw-r--r--   0        0        0     2687 2024-02-15 04:18:37.484684 ships-1.3.8/fields/gardens/ships/cadence/filter/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4059 2023-12-19 05:34:23.338811 ships-1.3.8/fields/gardens/ships/cadence/filter/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      843 2024-04-17 00:30:27.116287 ships-1.3.8/fields/gardens/ships/cadence/filter/_status/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0     1034 2024-04-17 00:30:26.956290 ships-1.3.8/fields/gardens/ships/cadence/filter/_status/__pycache__/status_2.cpython-310.pyc
+-rw-r--r--   0        0        0     1077 2024-04-17 00:30:27.000289 ships-1.3.8/fields/gardens/ships/cadence/filter/_status/__pycache__/status_3.cpython-310.pyc
+-rw-r--r--   0        0        0      533 2023-12-19 05:34:09.949917 ships-1.3.8/fields/gardens/ships/cadence/filter/_status/status_1.py
+-rw-r--r--   0        0        0      873 2023-12-19 05:34:09.960917 ships-1.3.8/fields/gardens/ships/cadence/filter/_status/status_2.py
+-rw-r--r--   0        0        0      961 2023-12-19 05:34:09.973917 ships-1.3.8/fields/gardens/ships/cadence/filter/_status/status_3.py
+-rw-r--r--   0        0        0      279 2023-11-10 20:08:24.789837 ships-1.3.8/fields/gardens/ships/cadence/orbits/orbits.r.html
+-rw-r--r--   0        0        0        2 2023-11-27 01:22:43.950708 ships-1.3.8/fields/gardens/ships/clique.py
+-rw-r--r--   0        0        0      117 2023-12-01 16:30:53.383074 ships-1.3.8/fields/gardens/ships/coms/coms.r.HTML
+-rw-r--r--   0        0        0      525 2023-12-01 14:37:22.097515 ships-1.3.8/fields/gardens/ships/coms/protocols/SSH/SSH.r.HTML
+-rw-r--r--   0        0        0      186 2023-12-01 21:53:45.724017 ships-1.3.8/fields/gardens/ships/coms/protocols/SSL/SSL.r.HTML
+-rw-r--r--   0        0        0        2 2023-12-01 16:29:57.831848 ships-1.3.8/fields/gardens/ships/coms/wall/wall.r.HTML
+-rw-r--r--   0        0        0      184 2023-12-19 05:34:10.022917 ships-1.3.8/fields/gardens/ships/cycle/__init__.py
+-rw-r--r--   0        0        0      420 2024-02-15 04:18:37.444684 ships-1.3.8/fields/gardens/ships/cycle/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      522 2023-12-19 05:34:23.357811 ships-1.3.8/fields/gardens/ships/cycle/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1850 2023-11-08 18:21:02.370631 ships-1.3.8/fields/gardens/ships/cycle/__pycache__/loops.cpython-311.pyc
+-rw-r--r--   0        0        0      878 2023-11-08 18:22:42.926530 ships-1.3.8/fields/gardens/ships/cycle/__pycache__/params.cpython-311.pyc
+-rw-r--r--   0        0        0      883 2023-11-08 18:27:36.336319 ships-1.3.8/fields/gardens/ships/cycle/__pycache__/presents.cpython-311.pyc
+-rw-r--r--   0        0        0      610 2024-04-09 19:03:39.047772 ships-1.3.8/fields/gardens/ships/cycle/cycle.S.HTML
+-rw-r--r--   0        0        0     1715 2024-04-09 18:50:19.806097 ships-1.3.8/fields/gardens/ships/cycle/loops/__init__.py
+-rw-r--r--   0        0        0     1233 2024-04-16 02:27:49.074085 ships-1.3.8/fields/gardens/ships/cycle/loops/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2009 2024-01-06 04:04:08.042839 ships-1.3.8/fields/gardens/ships/cycle/loops/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      915 2024-04-17 00:30:27.124287 ships-1.3.8/fields/gardens/ships/cycle/loops/__pycache__/status_2.cpython-310.pyc
+-rw-r--r--   0        0        0      906 2024-04-17 00:30:27.148287 ships-1.3.8/fields/gardens/ships/cycle/loops/__pycache__/status_3.cpython-310.pyc
+-rw-r--r--   0        0        0      970 2024-04-17 00:30:27.004289 ships-1.3.8/fields/gardens/ships/cycle/loops/__pycache__/status_4.cpython-310.pyc
+-rw-r--r--   0        0        0        6 2023-11-12 17:53:20.244810 ships-1.3.8/fields/gardens/ships/cycle/loops/loops.s.HTML
+-rw-r--r--   0        0        0      711 2023-12-19 05:47:03.340798 ships-1.3.8/fields/gardens/ships/cycle/loops/status_2.py
+-rw-r--r--   0        0        0      622 2023-12-19 05:34:10.055916 ships-1.3.8/fields/gardens/ships/cycle/loops/status_3.py
+-rw-r--r--   0        0        0      716 2023-12-19 05:34:10.066916 ships-1.3.8/fields/gardens/ships/cycle/loops/status_4.py
+-rw-r--r--   0        0        0      658 2023-11-12 18:07:23.961957 ships-1.3.8/fields/gardens/ships/cycle/params/__init__.py
+-rw-r--r--   0        0        0      672 2024-02-15 04:18:37.476684 ships-1.3.8/fields/gardens/ships/cycle/params/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      968 2023-11-12 18:07:25.924936 ships-1.3.8/fields/gardens/ships/cycle/params/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      679 2024-04-17 00:30:26.880291 ships-1.3.8/fields/gardens/ships/cycle/params/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0      758 2024-04-17 00:30:27.096288 ships-1.3.8/fields/gardens/ships/cycle/params/__pycache__/status_2.cpython-310.pyc
+-rw-r--r--   0        0        0      433 2023-12-19 05:34:10.077916 ships-1.3.8/fields/gardens/ships/cycle/params/status_1.py
+-rw-r--r--   0        0        0      536 2023-12-19 05:34:10.088916 ships-1.3.8/fields/gardens/ships/cycle/params/status_2.py
+-rw-r--r--   0        0        0      940 2024-01-06 04:12:45.342082 ships-1.3.8/fields/gardens/ships/cycle/params_2/__init__.py
+-rw-r--r--   0        0        0      873 2024-02-15 04:18:40.316651 ships-1.3.8/fields/gardens/ships/cycle/params_2/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1289 2024-01-06 04:13:16.981731 ships-1.3.8/fields/gardens/ships/cycle/params_2/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1005 2024-04-17 00:30:27.088288 ships-1.3.8/fields/gardens/ships/cycle/params_2/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0      853 2023-12-28 20:22:31.165818 ships-1.3.8/fields/gardens/ships/cycle/params_2/status_1.py
+-rw-r--r--   0        0        0      313 2023-12-19 05:34:10.129916 ships-1.3.8/fields/gardens/ships/cycle/presents/__init__.py
+-rw-r--r--   0        0        0      671 2024-02-15 04:18:37.444684 ships-1.3.8/fields/gardens/ships/cycle/presents/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      893 2023-12-19 05:34:23.627809 ships-1.3.8/fields/gardens/ships/cycle/presents/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1175 2023-12-19 05:34:10.140916 ships-1.3.8/fields/gardens/ships/flow/demux_mux/__init__.py
+-rw-r--r--   0        0        0     1555 2024-02-15 04:18:37.496683 ships-1.3.8/fields/gardens/ships/flow/demux_mux/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2435 2023-12-19 05:34:23.355811 ships-1.3.8/fields/gardens/ships/flow/demux_mux/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1448 2024-04-17 00:30:26.780292 ships-1.3.8/fields/gardens/ships/flow/demux_mux/_status/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0     1056 2023-12-19 05:34:10.152916 ships-1.3.8/fields/gardens/ships/flow/demux_mux/_status/status_1.py
+-rw-r--r--   0        0        0      334 2023-11-27 01:18:22.607776 ships-1.3.8/fields/gardens/ships/flow/demux_mux/demux_mux.r.html
+-rw-r--r--   0        0        0      830 2023-12-19 05:34:10.162916 ships-1.3.8/fields/gardens/ships/flow/demux_mux2/__init__.py
+-rw-r--r--   0        0        0      830 2024-02-15 04:18:37.472684 ships-1.3.8/fields/gardens/ships/flow/demux_mux2/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1187 2023-12-19 05:34:23.355811 ships-1.3.8/fields/gardens/ships/flow/demux_mux2/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      805 2024-04-17 00:30:27.000289 ships-1.3.8/fields/gardens/ships/flow/demux_mux2/_status/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0      515 2023-12-19 05:34:10.174915 ships-1.3.8/fields/gardens/ships/flow/demux_mux2/_status/status_1.py
+-rw-r--r--   0        0        0      285 2023-11-08 16:55:45.185683 ships-1.3.8/fields/gardens/ships/flow/flow.s.HTML
+-rw-r--r--   0        0        0     1428 2024-04-24 00:50:48.072605 ships-1.3.8/fields/gardens/ships/flow/simultaneous/__init__.py
+-rw-r--r--   0        0        0     2421 2024-04-24 04:19:26.091082 ships-1.3.8/fields/gardens/ships/flow/simultaneous_v2/__init__.py
+-rw-r--r--   0        0        0     1898 2024-04-24 04:23:09.031334 ships-1.3.8/fields/gardens/ships/flow/simultaneous_v2/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1125 2024-04-24 04:18:22.507783 ships-1.3.8/fields/gardens/ships/flow/simultaneous_v2/_status/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0     1161 2024-04-24 04:18:18.755824 ships-1.3.8/fields/gardens/ships/flow/simultaneous_v2/_status/status_1.py
+-rw-r--r--   0        0        0      919 2024-01-19 20:43:25.697218 ships-1.3.8/fields/gardens/ships/formats/ISO/ISO.s.HTML
+-rw-r--r--   0        0        0     6927 2023-11-18 21:15:34.850274 ships-1.3.8/fields/gardens/ships/glamour/UTF8/one.HTML
+-rw-r--r--   0        0        0      814 2024-02-15 04:18:37.464684 ships-1.3.8/fields/gardens/ships/insure/__pycache__/equalities.cpython-310.pyc
+-rw-r--r--   0        0        0     1249 2023-12-19 05:34:23.625809 ships-1.3.8/fields/gardens/ships/insure/__pycache__/equalities.cpython-311.pyc
+-rw-r--r--   0        0        0      694 2023-11-22 19:22:56.114817 ships-1.3.8/fields/gardens/ships/insure/__pycache__/equality.cpython-311.pyc
+-rw-r--r--   0        0        0      555 2024-04-17 00:30:26.724293 ships-1.3.8/fields/gardens/ships/insure/__pycache__/status_equalitites_1.cpython-310.pyc
+-rw-r--r--   0        0        0      690 2023-12-19 05:34:10.189915 ships-1.3.8/fields/gardens/ships/insure/equalities.py
+-rw-r--r--   0        0        0      231 2023-12-19 05:34:10.201915 ships-1.3.8/fields/gardens/ships/insure/equality.py
+-rw-r--r--   0        0        0      371 2023-12-19 05:34:10.213915 ships-1.3.8/fields/gardens/ships/insure/status_equalitites_1.py
+-rw-r--r--   0        0        0     1108 2024-03-30 19:19:49.968672 ships-1.3.8/fields/gardens/ships/module.MD
+-rw-r--r--   0        0        0      626 2024-03-17 02:48:33.516262 ships-1.3.8/fields/gardens/ships/modules/exceptions/__pycache__/parse.cpython-310.pyc
+-rw-r--r--   0        0        0      884 2023-12-19 05:34:23.635809 ships-1.3.8/fields/gardens/ships/modules/exceptions/__pycache__/parse.cpython-311.pyc
+-rw-r--r--   0        0        0      221 2023-11-29 22:52:11.709614 ships-1.3.8/fields/gardens/ships/modules/exceptions/custom/__init__.py
+-rw-r--r--   0        0        0      445 2024-03-10 22:49:28.895330 ships-1.3.8/fields/gardens/ships/modules/exceptions/parse.py
+-rw-r--r--   0        0        0      845 2023-12-19 05:34:10.235915 ships-1.3.8/fields/gardens/ships/modules/fasten/__init__.py
+-rw-r--r--   0        0        0      858 2024-02-15 04:18:37.508683 ships-1.3.8/fields/gardens/ships/modules/fasten/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1330 2023-12-19 05:34:23.630809 ships-1.3.8/fields/gardens/ships/modules/fasten/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      351 2024-02-15 04:18:37.564683 ships-1.3.8/fields/gardens/ships/modules/fasten/_status/__pycache__/example.cpython-310.pyc
+-rw-r--r--   0        0        0      415 2023-10-31 18:11:04.388642 ships-1.3.8/fields/gardens/ships/modules/fasten/_status/__pycache__/example.cpython-311.pyc
+-rw-r--r--   0        0        0      447 2024-02-15 04:18:37.508683 ships-1.3.8/fields/gardens/ships/modules/fasten/_status/__pycache__/example_caller.cpython-310.pyc
+-rw-r--r--   0        0        0      587 2023-12-19 05:34:23.632809 ships-1.3.8/fields/gardens/ships/modules/fasten/_status/__pycache__/example_caller.cpython-311.pyc
+-rw-r--r--   0        0        0      522 2024-04-17 00:30:26.704293 ships-1.3.8/fields/gardens/ships/modules/fasten/_status/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0       46 2023-10-31 18:06:14.891051 ships-1.3.8/fields/gardens/ships/modules/fasten/_status/example.py
+-rw-r--r--   0        0        0      121 2023-12-19 05:34:10.246915 ships-1.3.8/fields/gardens/ships/modules/fasten/_status/example_caller.py
+-rw-r--r--   0        0        0      255 2023-12-19 05:34:10.257915 ships-1.3.8/fields/gardens/ships/modules/fasten/_status/status_1.py
+-rw-r--r--   0        0        0      254 2023-11-28 04:58:18.174208 ships-1.3.8/fields/gardens/ships/modules/import/examples/__pycache__/example_1_module.cpython-311.pyc
+-rw-r--r--   0        0        0      364 2023-11-28 05:02:32.938052 ships-1.3.8/fields/gardens/ships/modules/import/examples/example_1.py
+-rw-r--r--   0        0        0        0 2023-11-28 04:57:58.030378 ships-1.3.8/fields/gardens/ships/modules/import/examples/example_1_module.py
+-rw-r--r--   0        0        0      382 2023-11-30 01:01:28.804136 ships-1.3.8/fields/gardens/ships/modules/import/import.r.HTML
+-rw-r--r--   0        0        0      679 2023-11-27 01:32:02.156155 ships-1.3.8/fields/gardens/ships/modules/print/print.s.HTML
+-rw-r--r--   0        0        0       59 2023-12-17 22:23:07.000749 ships-1.3.8/fields/gardens/ships/modules/string/NLP/NLP.s.HTML
+-rw-r--r--   0        0        0      265 2023-11-12 18:56:01.444149 ships-1.3.8/fields/gardens/ships/modules/string/end_of_string_is.py
+-rw-r--r--   0        0        0       93 2023-12-17 22:25:39.567979 ships-1.3.8/fields/gardens/ships/modules/string/sayings/sayings.s.HTML
+-rw-r--r--   0        0        0      223 2023-12-01 04:01:32.322888 ships-1.3.8/fields/gardens/ships/paths/caller.py
+-rw-r--r--   0        0        0     3453 2024-02-15 05:14:15.432421 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/__init__.py
+-rw-r--r--   0        0        0     2534 2024-02-15 05:15:22.147687 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3944 2023-12-19 05:34:23.327811 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      956 2024-04-17 00:30:26.768292 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/_status/1/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2023-09-26 17:01:19.501305 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/_status/1/directories/EQ_1/1.HTML
+-rw-r--r--   0        0        0        0 2023-09-26 17:01:24.477254 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/_status/1/directories/EQ_2/1.HTML
+-rw-r--r--   0        0        0      587 2024-02-15 05:03:56.927189 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/_status/1/status_1.py
+-rw-r--r--   0        0        0     1018 2024-04-17 00:30:26.772292 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/_status/2/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2023-09-26 17:12:57.126345 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/_status/2/directories/EQ_1/1/1.HTML
+-rw-r--r--   0        0        0        0 2023-09-26 17:12:39.434518 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/_status/2/directories/EQ_1/1.HTML
+-rw-r--r--   0        0        0        0 2023-09-26 17:13:01.703300 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/_status/2/directories/EQ_2/1/2.HTML
+-rw-r--r--   0        0        0        0 2023-09-26 17:12:42.709486 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/_status/2/directories/EQ_2/2.HTML
+-rw-r--r--   0        0        0      682 2023-12-19 05:34:10.289914 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/_status/2/status_1.py
+-rw-r--r--   0        0        0        3 2024-02-15 04:09:56.998834 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/clique.py
+-rw-r--r--   0        0        0     1225 2023-09-26 17:25:34.940919 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/ADD_DIFFERENT_CONTENTS.cpython-311.pyc
+-rw-r--r--   0        0        0     1082 2023-09-26 17:24:58.886273 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/ADD_DIFFERENT_PATHS.cpython-311.pyc
+-rw-r--r--   0        0        0      767 2023-09-26 17:19:39.017407 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/GET_DIRECTORIES.cpython-311.pyc
+-rw-r--r--   0        0        0      868 2023-09-26 17:20:39.552814 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/GET_SAME_DIRECTORIES.cpython-311.pyc
+-rw-r--r--   0        0        0      435 2023-09-26 17:18:11.864261 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/IS_DIR.cpython-311.pyc
+-rw-r--r--   0        0        0      822 2024-02-15 04:17:31.001458 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/add_different_contents.cpython-310.pyc
+-rw-r--r--   0        0        0     1287 2023-12-03 23:12:22.567309 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/add_different_contents.cpython-311.pyc
+-rw-r--r--   0        0        0      738 2024-02-15 04:17:31.001458 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/add_different_paths.cpython-310.pyc
+-rw-r--r--   0        0        0     1115 2023-12-03 23:12:22.567309 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/add_different_paths.cpython-311.pyc
+-rw-r--r--   0        0        0      589 2024-02-15 04:17:31.001458 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/get_directories.cpython-310.pyc
+-rw-r--r--   0        0        0      800 2023-12-03 23:12:22.566310 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/get_directories.cpython-311.pyc
+-rw-r--r--   0        0        0      650 2024-02-15 04:17:31.001458 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/get_same_directories.cpython-310.pyc
+-rw-r--r--   0        0        0      901 2023-12-03 23:12:22.566310 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/get_same_directories.cpython-311.pyc
+-rw-r--r--   0        0        0      393 2024-02-15 04:17:30.997458 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/is_dir.cpython-310.pyc
+-rw-r--r--   0        0        0      469 2023-12-03 23:12:22.566310 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/is_dir.cpython-311.pyc
+-rw-r--r--   0        0        0      702 2023-12-03 23:10:11.791819 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/add_different_contents.py
+-rw-r--r--   0        0        0      575 2023-12-03 23:10:11.805819 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/add_different_paths.py
+-rw-r--r--   0        0        0      291 2023-12-03 23:10:11.818818 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/get_directories.py
+-rw-r--r--   0        0        0      431 2023-12-03 23:10:11.830819 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/get_same_directories.py
+-rw-r--r--   0        0        0       70 2023-12-03 21:57:50.893795 ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/is_dir.py
+-rw-r--r--   0        0        0      165 2023-12-19 05:34:10.300914 ships-1.3.8/fields/gardens/ships/paths/directory/deallocate/__init__.py
+-rw-r--r--   0        0        0      494 2024-02-15 04:18:37.464684 ships-1.3.8/fields/gardens/ships/paths/directory/deallocate/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      585 2023-12-19 05:34:23.325811 ships-1.3.8/fields/gardens/ships/paths/directory/deallocate/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      142 2023-10-13 23:54:15.372867 ships-1.3.8/fields/gardens/ships/paths/directory/directory.html
+-rw-r--r--   0        0        0     2162 2024-04-07 02:50:44.194867 ships-1.3.8/fields/gardens/ships/paths/directory/equalize/__init__.py
+-rw-r--r--   0        0        0     2035 2024-04-07 02:50:55.966733 ships-1.3.8/fields/gardens/ships/paths/directory/equalize/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2556 2024-01-14 00:41:51.174597 ships-1.3.8/fields/gardens/ships/paths/directory/equalize/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1461 2024-04-17 00:30:26.756292 ships-1.3.8/fields/gardens/ships/paths/directory/equalize/_status/1/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0       10 2023-10-14 00:40:16.169744 ships-1.3.8/fields/gardens/ships/paths/directory/equalize/_status/1/start/1/1.py
+-rw-r--r--   0        0        0        7 2023-10-14 00:57:00.845808 ships-1.3.8/fields/gardens/ships/paths/directory/equalize/_status/1/start/2/2.txt
+-rw-r--r--   0        0        0        4 2023-10-14 00:56:55.910862 ships-1.3.8/fields/gardens/ships/paths/directory/equalize/_status/1/start/3/3.txt
+-rw-r--r--   0        0        0     1387 2024-03-30 03:49:06.306137 ships-1.3.8/fields/gardens/ships/paths/directory/equalize/_status/1/status_1.py
+-rw-r--r--   0        0        0     1392 2024-04-17 00:30:26.728293 ships-1.3.8/fields/gardens/ships/paths/directory/equalize/_status/2/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0       10 2023-10-14 00:40:16.169744 ships-1.3.8/fields/gardens/ships/paths/directory/equalize/_status/2/start/1/1.py
+-rw-r--r--   0        0        0        7 2023-10-14 00:57:00.845808 ships-1.3.8/fields/gardens/ships/paths/directory/equalize/_status/2/start/2/2.txt
+-rw-r--r--   0        0        0        0 2023-10-14 01:31:12.050509 ships-1.3.8/fields/gardens/ships/paths/directory/equalize/_status/2/start/2/55/55.txt
+-rw-r--r--   0        0        0        4 2023-10-14 00:56:55.910862 ships-1.3.8/fields/gardens/ships/paths/directory/equalize/_status/2/start/3/3.txt
+-rw-r--r--   0        0        0        0 2023-10-14 01:31:02.205616 ships-1.3.8/fields/gardens/ships/paths/directory/equalize/_status/2/start/3/9/9.txt
+-rw-r--r--   0        0        0     1284 2023-12-19 05:34:10.344914 ships-1.3.8/fields/gardens/ships/paths/directory/equalize/_status/2/status_1.py
+-rw-r--r--   0        0        0      101 2023-10-13 23:54:40.745591 ships-1.3.8/fields/gardens/ships/paths/directory/equalize/equalize.S.HTML
+-rw-r--r--   0        0        0     1598 2024-04-12 21:58:19.908257 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/__init__.py
+-rw-r--r--   0        0        0     1239 2024-04-16 02:27:49.606078 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2655 2023-12-19 05:34:23.624809 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1512 2024-04-17 00:30:26.804292 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/1.contents/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0        8 2023-11-09 18:10:08.040409 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/1.contents/cryo/1/example.html
+-rw-r--r--   0        0        0     1113 2024-03-30 05:25:31.843636 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/1.contents/status_1.py
+-rw-r--r--   0        0        0     1708 2024-04-17 00:30:27.056288 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/2.contents/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0        8 2023-11-09 18:10:08.040409 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/2.contents/cryo/1/example.html
+-rw-r--r--   0        0        0       22 2024-03-30 04:06:34.621842 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/2.contents/cryo/S.HTML
+-rw-r--r--   0        0        0       16 2024-03-30 04:06:46.557705 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/2.contents/cryo/another_place/place.HTML
+-rw-r--r--   0        0        0     1349 2024-03-30 05:25:43.287496 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/2.contents/status_1.py
+-rw-r--r--   0        0        0       10 2023-10-14 00:40:16.169744 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/3.contents_and_paths/temp/1/1.py
+-rw-r--r--   0        0        0        0 2024-03-30 05:00:29.274092 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/3.contents_and_paths/temp/1.txt
+-rw-r--r--   0        0        0        7 2023-10-14 00:57:00.845808 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/3.contents_and_paths/temp/2/2.txt
+-rw-r--r--   0        0        0        0 2023-10-14 01:31:12.050509 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/3.contents_and_paths/temp/2/55/55.txt
+-rw-r--r--   0        0        0        4 2023-10-14 00:56:55.910861 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/3.contents_and_paths/temp/3/3.txt
+-rw-r--r--   0        0        0        0 2023-10-14 01:31:02.205616 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/3.contents_and_paths/temp/3/9/9.txt
+-rw-r--r--   0        0        0       10 2023-10-14 00:40:16.169744 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/3.contents_and_paths/temp/symlink_to_1/1.py
+-rw-r--r--   0        0        0        0 2024-03-30 05:00:29.274092 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/3.contents_and_paths/temp/symlink_to_1.txt
+-rw-r--r--   0        0        0      196 2024-03-30 04:06:11.050111 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/field.S.HTML
+-rw-r--r--   0        0        0      115 2023-10-21 23:43:14.421112 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/in_path.py
+-rw-r--r--   0        0        0     3636 2024-04-16 02:26:41.806881 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/__init__.py
+-rw-r--r--   0        0        0     2426 2024-04-16 02:27:49.110084 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2655 2023-12-19 05:34:23.624809 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1514 2024-04-17 00:30:27.056288 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/1.contents/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0        8 2023-11-09 18:10:08.040409 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/1.contents/cryo/example.html
+-rw-r--r--   0        0        0     1117 2024-03-30 18:35:45.388509 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/1.contents/status_1.py
+-rw-r--r--   0        0        0     1733 2024-04-17 00:30:26.924290 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/2.contents/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0        8 2023-11-09 18:10:08.040409 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/2.contents/cryo/1/example.html
+-rw-r--r--   0        0        0       22 2024-03-30 04:06:34.621841 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/2.contents/cryo/S.HTML
+-rw-r--r--   0        0        0       16 2024-03-30 04:06:46.557705 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/2.contents/cryo/another_place/place.HTML
+-rw-r--r--   0        0        0     1358 2024-03-30 19:02:42.946268 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/2.contents/status_1.py
+-rw-r--r--   0        0        0     2128 2024-04-17 00:30:27.112287 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0       10 2023-10-14 00:40:16.169744 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo/1/1.py
+-rw-r--r--   0        0        0        0 2024-03-30 05:00:29.274092 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo/1.txt
+-rw-r--r--   0        0        0        7 2023-10-14 00:57:00.845808 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo/2/2.txt
+-rw-r--r--   0        0        0        0 2023-10-14 01:31:12.050509 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo/2/55/55.txt
+-rw-r--r--   0        0        0        4 2023-10-14 00:56:55.910861 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo/3/3.txt
+-rw-r--r--   0        0        0        0 2023-10-14 01:31:02.205616 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo/3/9/9.txt
+-rw-r--r--   0        0        0       15 2024-03-30 18:35:01.213003 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo/txt/something.txt
+-rw-r--r--   0        0        0       10 2023-10-14 00:40:16.169744 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo_proceeds/1/1.py
+-rw-r--r--   0        0        0        0 2024-03-30 05:00:29.274092 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo_proceeds/1.the_txt
+-rw-r--r--   0        0        0        7 2023-10-14 00:57:00.845808 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo_proceeds/2/2.the_txt
+-rw-r--r--   0        0        0        0 2023-10-14 01:31:12.050509 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo_proceeds/2/55/55.the_txt
+-rw-r--r--   0        0        0        4 2023-10-14 00:56:55.910861 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo_proceeds/3/3.the_txt
+-rw-r--r--   0        0        0        0 2023-10-14 01:31:02.205616 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo_proceeds/3/9/9.the_txt
+-rw-r--r--   0        0        0       10 2023-10-14 00:40:16.169744 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo_proceeds/symlink_to_1/1.py
+-rw-r--r--   0        0        0        0 2024-03-30 05:00:29.274092 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo_proceeds/symlink_to_1.the_txt
+-rw-r--r--   0        0        0       19 2024-03-30 18:54:24.571904 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/cryo_proceeds/the_txt/something.the_txt
+-rw-r--r--   0        0        0     1881 2024-03-30 18:59:07.456706 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/status_1.py
+-rw-r--r--   0        0        0       10 2023-10-14 00:40:16.169744 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/temp/1/1.py
+-rw-r--r--   0        0        0        0 2024-03-30 05:00:29.274092 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/temp/1.the_txt
+-rw-r--r--   0        0        0        7 2023-10-14 00:57:00.845808 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/temp/2/2.the_txt
+-rw-r--r--   0        0        0        0 2023-10-14 01:31:12.050509 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/temp/2/55/55.the_txt
+-rw-r--r--   0        0        0        4 2023-10-14 00:56:55.910861 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/temp/3/3.the_txt
+-rw-r--r--   0        0        0        0 2023-10-14 01:31:02.205616 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/temp/3/9/9.the_txt
+-rw-r--r--   0        0        0       10 2023-10-14 00:40:16.169744 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/temp/symlink_to_1/1.py
+-rw-r--r--   0        0        0        0 2024-03-30 05:00:29.274092 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/temp/symlink_to_1.the_txt
+-rw-r--r--   0        0        0       19 2024-04-24 04:23:09.443319 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/temp/the_txt/something.the_txt
+-rw-r--r--   0        0        0      196 2024-03-30 04:06:11.050111 ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/field.S.HTML
+-rw-r--r--   0        0        0      781 2023-10-21 23:50:37.854518 ships-1.3.8/fields/gardens/ships/paths/directory/for_each_path/__init__.py
+-rw-r--r--   0        0        0     1797 2023-12-19 05:34:10.383914 ships-1.3.8/fields/gardens/ships/paths/directory/rsync/__init__.py
+-rw-r--r--   0        0        0     1768 2024-02-15 04:18:37.480684 ships-1.3.8/fields/gardens/ships/paths/directory/rsync/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2500 2023-12-19 05:34:23.330811 ships-1.3.8/fields/gardens/ships/paths/directory/rsync/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      974 2024-03-30 18:50:21.894647 ships-1.3.8/fields/gardens/ships/paths/directory/scan_tree/DFS.py
+-rw-r--r--   0        0        0     2200 2024-03-30 18:22:06.590291 ships-1.3.8/fields/gardens/ships/paths/directory/scan_tree/__init__.py
+-rw-r--r--   0        0        0     2032 2024-03-30 18:03:59.648399 ships-1.3.8/fields/gardens/ships/paths/directory/scan_tree/__init__v1.py
+-rw-r--r--   0        0        0      676 2024-03-30 18:50:27.118588 ships-1.3.8/fields/gardens/ships/paths/directory/scan_tree/__pycache__/DFS.cpython-310.pyc
+-rw-r--r--   0        0        0     1426 2024-03-30 18:22:08.390268 ships-1.3.8/fields/gardens/ships/paths/directory/scan_tree/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2076 2024-04-17 00:30:27.084288 ships-1.3.8/fields/gardens/ships/paths/directory/scan_tree/_status/1/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0       10 2023-10-14 00:40:16.169744 ships-1.3.8/fields/gardens/ships/paths/directory/scan_tree/_status/1/cryo/1/1.py
+-rw-r--r--   0        0        0        0 2024-03-30 05:00:29.274092 ships-1.3.8/fields/gardens/ships/paths/directory/scan_tree/_status/1/cryo/1.txt
+-rw-r--r--   0        0        0        7 2023-10-14 00:57:00.845808 ships-1.3.8/fields/gardens/ships/paths/directory/scan_tree/_status/1/cryo/2/2.txt
+-rw-r--r--   0        0        0        0 2023-10-14 01:31:12.050509 ships-1.3.8/fields/gardens/ships/paths/directory/scan_tree/_status/1/cryo/2/55/55.txt
+-rw-r--r--   0        0        0        4 2023-10-14 00:56:55.910861 ships-1.3.8/fields/gardens/ships/paths/directory/scan_tree/_status/1/cryo/3/3.txt
+-rw-r--r--   0        0        0        0 2023-10-14 01:31:02.205616 ships-1.3.8/fields/gardens/ships/paths/directory/scan_tree/_status/1/cryo/3/9/9.txt
+-rw-r--r--   0        0        0     3629 2024-03-30 19:04:59.464724 ships-1.3.8/fields/gardens/ships/paths/directory/scan_tree/_status/1/status_1.py
+-rw-r--r--   0        0        0     1343 2024-04-17 00:30:26.712293 ships-1.3.8/fields/gardens/ships/paths/directory/scan_tree/_status/2/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-03-30 17:46:36.128181 ships-1.3.8/fields/gardens/ships/paths/directory/scan_tree/_status/2/cryo.txt
+-rw-r--r--   0        0        0     1020 2024-03-30 19:04:22.217145 ships-1.3.8/fields/gardens/ships/paths/directory/scan_tree/_status/2/status_1.py
+-rw-r--r--   0        0        0     1212 2023-12-19 05:34:10.397914 ships-1.3.8/fields/gardens/ships/paths/directory/sense/__init__.py
+-rw-r--r--   0        0        0     1768 2024-02-15 04:18:37.444684 ships-1.3.8/fields/gardens/ships/paths/directory/sense/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2584 2023-12-19 05:34:23.331811 ships-1.3.8/fields/gardens/ships/paths/directory/sense/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1021 2024-04-17 00:30:26.844291 ships-1.3.8/fields/gardens/ships/paths/directory/sense/_status/1/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0      826 2024-03-30 05:18:51.408533 ships-1.3.8/fields/gardens/ships/paths/directory/sense/_status/1/status_1.py
+-rw-r--r--   0        0        0      763 2023-12-19 05:34:10.423913 ships-1.3.8/fields/gardens/ships/paths/directory/size/__init__.py
+-rw-r--r--   0        0        0     1116 2024-02-15 04:18:37.476684 ships-1.3.8/fields/gardens/ships/paths/directory/size/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1819 2023-12-19 05:34:23.329811 ships-1.3.8/fields/gardens/ships/paths/directory/size/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      947 2024-04-17 00:30:26.992289 ships-1.3.8/fields/gardens/ships/paths/directory/size/_status/1/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0       34 2023-12-03 23:22:28.062362 ships-1.3.8/fields/gardens/ships/paths/directory/size/_status/1/cryo/hyper.HTML
+-rw-r--r--   0        0        0      623 2023-12-19 05:34:10.435913 ships-1.3.8/fields/gardens/ships/paths/directory/size/_status/1/status_1.py
+-rw-r--r--   0        0        0      544 2023-12-19 05:34:10.447913 ships-1.3.8/fields/gardens/ships/paths/files/scan/JSON/__init__.py
+-rw-r--r--   0        0        0     1362 2023-11-09 20:55:25.502570 ships-1.3.8/fields/gardens/ships/paths/files/scan/JSON/__pycache__/JSON.cpython-311.pyc
+-rw-r--r--   0        0        0      928 2024-02-15 04:18:37.480684 ships-1.3.8/fields/gardens/ships/paths/files/scan/JSON/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1378 2023-12-19 05:34:23.647809 ships-1.3.8/fields/gardens/ships/paths/files/scan/JSON/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0       15 2023-11-09 20:50:52.710653 ships-1.3.8/fields/gardens/ships/paths/files/scan/JSON/cryo/example.JSON
+-rw-r--r--   0        0        0      868 2024-04-17 00:30:26.760292 ships-1.3.8/fields/gardens/ships/paths/files/scan/JSON/status/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0      534 2023-12-19 05:34:10.459913 ships-1.3.8/fields/gardens/ships/paths/files/scan/JSON/status/status_1.py
+-rw-r--r--   0        0        0      932 2023-10-13 23:36:51.568242 ships-1.3.8/fields/gardens/ships/paths/fs, rsync details.r.html
+-rw-r--r--   0        0        0      367 2023-10-13 23:35:46.146955 ships-1.3.8/fields/gardens/ships/paths/fs.r.html
+-rw-r--r--   0        0        0      934 2023-11-09 20:55:40.948395 ships-1.3.8/fields/gardens/ships/paths/path/__pycache__/relative.cpython-311.pyc
+-rw-r--r--   0        0        0      327 2023-12-19 05:34:10.470913 ships-1.3.8/fields/gardens/ships/paths/path/relative.py
+-rw-r--r--   0        0        0      396 2024-03-30 18:12:33.670409 ships-1.3.8/fields/gardens/ships/paths/variety/__init__.py
+-rw-r--r--   0        0        0      485 2024-03-30 18:15:40.351557 ships-1.3.8/fields/gardens/ships/paths/variety/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    12177 2024-01-23 00:01:37.980550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/ANSI.py
+-rw-r--r--   0        0        0    13419 2024-01-23 00:01:37.980550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/FSM.py
+-rw-r--r--   0        0        0     4089 2024-01-23 00:01:37.980550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__init__.py
+-rw-r--r--   0        0        0    19876 2024-01-23 00:01:37.984550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/ANSI.cpython-311.pyc
+-rw-r--r--   0        0        0    16297 2024-01-23 00:01:37.985550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/FSM.cpython-311.pyc
+-rw-r--r--   0        0        0     4220 2024-02-15 04:18:39.816656 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4382 2024-01-23 00:01:37.985550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1043 2024-01-23 00:01:37.985550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/_async.cpython-311.pyc
+-rw-r--r--   0        0        0     6850 2024-01-23 00:01:37.986550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/_async_pre_await.cpython-311.pyc
+-rw-r--r--   0        0        0     6975 2024-01-23 00:01:37.986550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/_async_w_await.cpython-311.pyc
+-rw-r--r--   0        0        0     1932 2024-02-15 04:18:39.820656 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0        0        0     2671 2024-01-23 00:01:37.987550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/exceptions.cpython-311.pyc
+-rw-r--r--   0        0        0     9145 2024-02-15 04:18:39.832656 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/expect.cpython-310.pyc
+-rw-r--r--   0        0        0    16905 2024-01-23 00:01:37.988550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/expect.cpython-311.pyc
+-rw-r--r--   0        0        0     7983 2024-01-23 00:01:37.989550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/fdpexpect.cpython-311.pyc
+-rw-r--r--   0        0        0     8932 2024-01-23 00:01:37.989550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/popen_spawn.cpython-311.pyc
+-rw-r--r--   0        0        0    32161 2024-02-15 04:18:39.852656 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/pty_spawn.cpython-310.pyc
+-rw-r--r--   0        0        0    44581 2024-01-23 00:01:37.992550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/pty_spawn.cpython-311.pyc
+-rw-r--r--   0        0        0    23360 2024-01-23 00:01:37.993550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/pxssh.cpython-311.pyc
+-rw-r--r--   0        0        0     7584 2024-01-23 00:01:37.994550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/replwrap.cpython-311.pyc
+-rw-r--r--   0        0        0     5856 2024-02-15 04:18:39.860656 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/run.cpython-310.pyc
+-rw-r--r--   0        0        0     7805 2024-01-23 00:01:37.994550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/run.cpython-311.pyc
+-rw-r--r--   0        0        0    21594 2024-01-23 00:01:37.996550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/screen.cpython-311.pyc
+-rw-r--r--   0        0        0     7302 2024-01-23 00:01:37.996550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/socket_pexpect.cpython-311.pyc
+-rw-r--r--   0        0        0    17837 2024-02-15 04:18:39.856656 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/spawnbase.cpython-310.pyc
+-rw-r--r--   0        0        0    25269 2024-01-23 00:01:37.998550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/spawnbase.cpython-311.pyc
+-rw-r--r--   0        0        0     3850 2024-02-15 04:18:39.824657 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0     6357 2024-01-23 00:01:37.999550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0      907 2024-01-23 00:01:37.980550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/_async.py
+-rw-r--r--   0        0        0     3465 2024-01-23 00:01:37.980550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/_async_pre_await.py
+-rw-r--r--   0        0        0     3802 2024-01-23 00:01:37.980550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/_async_w_await.py
+-rw-r--r--   0        0        0      419 2024-01-23 00:01:37.980550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/bashrc.sh
+-rw-r--r--   0        0        0     1068 2024-01-23 00:01:37.980550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/exceptions.py
+-rw-r--r--   0        0        0    13827 2024-01-23 00:01:37.981550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/expect.py
+-rw-r--r--   0        0        0     5991 2024-01-23 00:01:37.981550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/fdpexpect.py
+-rw-r--r--   0        0        0        4 2024-01-23 00:01:37.999550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/pexpect-4.9.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0      987 2024-01-23 00:01:37.982550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/pexpect-4.9.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     2463 2024-01-23 00:01:37.982550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/pexpect-4.9.0.dist-info/METADATA
+-rw-r--r--   0        0        0     2900 2024-01-23 00:01:38.000550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/pexpect-4.9.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2024-01-23 00:01:37.999550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/pexpect-4.9.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0      110 2024-01-23 00:01:37.982550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/pexpect-4.9.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        8 2024-01-23 00:01:37.982550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/pexpect-4.9.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     6159 2024-01-23 00:01:37.981550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/popen_spawn.py
+-rw-r--r--   0        0        0    37382 2024-01-23 00:01:37.981550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/pty_spawn.py
+-rw-r--r--   0        0        0    24445 2024-01-23 00:01:37.981550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/pxssh.py
+-rw-r--r--   0        0        0     5951 2024-01-23 00:01:37.981550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/replwrap.py
+-rw-r--r--   0        0        0     6629 2024-01-23 00:01:37.981550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/run.py
+-rw-r--r--   0        0        0    13704 2024-01-23 00:01:37.982550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/screen.py
+-rw-r--r--   0        0        0     4814 2024-01-23 00:01:37.982550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/socket_pexpect.py
+-rw-r--r--   0        0        0    21685 2024-01-23 00:01:37.982550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/spawnbase.py
+-rw-r--r--   0        0        0     6019 2024-01-23 00:01:37.982550 ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/utils.py
+-rw-r--r--   0        0        0     1046 2024-02-15 04:18:41.940632 ships-1.3.8/fields/gardens/ships/ports/__pycache__/available.cpython-310.pyc
+-rw-r--r--   0        0        0     1616 2023-12-19 05:34:24.854799 ships-1.3.8/fields/gardens/ships/ports/__pycache__/available.cpython-311.pyc
+-rw-r--r--   0        0        0      638 2024-02-15 04:18:41.940632 ships-1.3.8/fields/gardens/ships/ports/__pycache__/claimed.cpython-310.pyc
+-rw-r--r--   0        0        0      938 2023-12-19 05:34:24.854799 ships-1.3.8/fields/gardens/ships/ports/__pycache__/claimed.cpython-311.pyc
+-rw-r--r--   0        0        0      606 2024-04-17 00:30:27.060288 ships-1.3.8/fields/gardens/ships/ports/_status/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0      507 2023-12-19 05:34:10.482913 ships-1.3.8/fields/gardens/ships/ports/_status/status_1.py
+-rw-r--r--   0        0        0      983 2023-12-19 05:34:10.496913 ships-1.3.8/fields/gardens/ships/ports/available.py
+-rw-r--r--   0        0        0      498 2023-12-19 05:34:10.507913 ships-1.3.8/fields/gardens/ships/ports/claimed.py
+-rw-r--r--   0        0        0      631 2023-12-19 05:34:10.519913 ships-1.3.8/fields/gardens/ships/ports/find_multiple/__init__.py
+-rw-r--r--   0        0        0      856 2024-02-15 04:18:41.936632 ships-1.3.8/fields/gardens/ships/ports/find_multiple/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1308 2023-12-19 05:34:24.854799 ships-1.3.8/fields/gardens/ships/ports/find_multiple/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      666 2024-04-17 00:30:27.080288 ships-1.3.8/fields/gardens/ships/ports/find_multiple/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0      419 2023-12-19 05:34:10.531913 ships-1.3.8/fields/gardens/ships/ports/find_multiple/status_1.py
+-rw-r--r--   0        0        0     1756 2024-01-23 00:49:41.930690 ships-1.3.8/fields/gardens/ships/process/multi/__init__.py
+-rw-r--r--   0        0        0     2030 2024-02-15 04:18:40.024654 ships-1.3.8/fields/gardens/ships/process/multi/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3162 2024-01-23 00:49:44.726658 ships-1.3.8/fields/gardens/ships/process/multi/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      891 2024-04-17 00:30:27.212286 ships-1.3.8/fields/gardens/ships/process/multi/_status/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0     1034 2024-04-17 00:30:27.240285 ships-1.3.8/fields/gardens/ships/process/multi/_status/__pycache__/status_2.cpython-310.pyc
+-rw-r--r--   0        0        0      851 2023-12-19 05:34:10.553912 ships-1.3.8/fields/gardens/ships/process/multi/_status/status_1.py
+-rw-r--r--   0        0        0      923 2024-01-23 03:58:21.718356 ships-1.3.8/fields/gardens/ships/process/multi/_status/status_2.py
+-rw-r--r--   0        0        0     3733 2024-01-23 04:02:43.996412 ships-1.3.8/fields/gardens/ships/process/multi_2/__init__.py
+-rw-r--r--   0        0        0     2725 2024-02-15 04:18:39.972655 ships-1.3.8/fields/gardens/ships/process/multi_2/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4843 2024-01-23 04:02:57.086266 ships-1.3.8/fields/gardens/ships/process/multi_2/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1536 2024-04-17 00:30:27.036288 ships-1.3.8/fields/gardens/ships/process/multi_2/_status/2/__pycache__/status_2.cpython-310.pyc
+-rw-r--r--   0        0        0      180 2024-01-22 23:55:08.820853 ships-1.3.8/fields/gardens/ships/process/multi_2/_status/2/script.py
+-rw-r--r--   0        0        0     1429 2024-01-23 04:15:28.615832 ships-1.3.8/fields/gardens/ships/process/multi_2/_status/2/status_2.py
+-rw-r--r--   0        0        0     1241 2024-04-17 00:30:26.936290 ships-1.3.8/fields/gardens/ships/process/multi_2/_status/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0     1005 2024-01-23 03:59:33.397551 ships-1.3.8/fields/gardens/ships/process/multi_2/_status/status_1.py
+-rw-r--r--   0        0        0     1605 2024-01-23 04:06:55.382592 ships-1.3.8/fields/gardens/ships/process/start/__init__.py
+-rw-r--r--   0        0        0     1395 2024-02-15 04:18:39.816656 ships-1.3.8/fields/gardens/ships/process/start/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2026 2024-01-23 04:07:13.569387 ships-1.3.8/fields/gardens/ships/process/start/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    69632 2024-01-23 03:07:00.507890 ships-1.3.8/fields/gardens/ships/process/start/_status/.coverage
+-rw-r--r--   0        0        0    69632 2024-01-23 04:02:47.177377 ships-1.3.8/fields/gardens/ships/process/start/_status/.status_1_coverage
+-rw-r--r--   0        0        0    53248 2024-01-23 01:43:21.048331 ships-1.3.8/fields/gardens/ships/process/start/_status/2/.coverage
+-rw-r--r--   0        0        0     1568 2024-04-17 00:30:26.896290 ships-1.3.8/fields/gardens/ships/process/start/_status/2/__pycache__/status_2.cpython-310.pyc
+-rw-r--r--   0        0        0      160 2024-01-23 01:46:12.526385 ships-1.3.8/fields/gardens/ships/process/start/_status/2/script.py
+-rw-r--r--   0        0        0     1495 2024-01-23 04:15:44.186657 ships-1.3.8/fields/gardens/ships/process/start/_status/2/status_2.py
+-rw-r--r--   0        0        0     1546 2024-04-17 00:30:27.016289 ships-1.3.8/fields/gardens/ships/process/start/_status/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0     1169 2024-01-23 04:07:00.762531 ships-1.3.8/fields/gardens/ships/process/start/_status/status_1.py
+-rw-r--r--   0        0        0      828 2024-02-15 04:18:40.124653 ships-1.3.8/fields/gardens/ships/process/start/parts/__pycache__/awareness.cpython-310.pyc
+-rw-r--r--   0        0        0     1623 2024-01-23 03:06:26.360273 ships-1.3.8/fields/gardens/ships/process/start/parts/__pycache__/awareness.cpython-311.pyc
+-rw-r--r--   0        0        0      647 2024-02-15 04:18:40.124653 ships-1.3.8/fields/gardens/ships/process/start/parts/__pycache__/returns.cpython-310.pyc
+-rw-r--r--   0        0        0      842 2024-01-23 04:07:13.655386 ships-1.3.8/fields/gardens/ships/process/start/parts/__pycache__/returns.cpython-311.pyc
+-rw-r--r--   0        0        0      916 2024-01-23 03:03:06.613515 ships-1.3.8/fields/gardens/ships/process/start/parts/awareness.py
+-rw-r--r--   0        0        0      486 2024-01-23 04:06:27.768901 ships-1.3.8/fields/gardens/ships/process/start/parts/returns.py
+-rw-r--r--   0        0        0       69 2023-12-19 05:34:10.556912 ships-1.3.8/fields/gardens/ships/revenue.py
+-rw-r--r--   0        0        0        8 2023-12-19 05:32:53.977518 ships-1.3.8/fields/gardens/ships/ships.s.HTML
+-rw-r--r--   0        0        0      584 2024-04-24 04:24:26.404615 ships-1.3.8/pyproject.toml
+-rw-r--r--   0        0        0     1108 2024-03-30 19:19:57.188600 ships-1.3.8/readme.md
+-rw-r--r--   0        0        0      884 2024-04-17 00:31:00.159834 ships-1.3.8/ships.S.HTML
+-rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 ships-1.3.8/PKG-INFO
```

### Comparing `ships-1.2.8/fields/gardens/ships/__init__.py` & `ships-1.3.8/fields/gardens/ships/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_clique/__init__.py` & `ships-1.3.8/fields/gardens/ships/_clique/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_clique/__pycache__/__init__.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/_clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_license/licenses/gpl-3.0-standalone.html` & `ships-1.3.8/fields/gardens/ships/_license/licenses/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/.coverage` & `ships-1.3.8/fields/gardens/ships/_status/.coverage`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/DB/records.json` & `ships-1.3.8/fields/gardens/ships/_status/DB/records.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772313296903461%*

 * *Differences: {"'_default'": "{'525': OrderedDict([('paths', [OrderedDict([('path', "*

 * *               "'modules/fasten/_status/status_1.py'), ('empty', False), ('parsed', True), "*

 * *               "('stats', OrderedDict([('passes', 1), ('alarms', 0)])), ('checks', "*

 * *               "[OrderedDict([('check', 'fastener 1'), ('passed', True), ('elapsed', "*

 * *               "[0.03455425500214915, 'seconds'])])])]), OrderedDict([('path', "*

 * *               "'insure/status_equalitites_1.py'), ('empty', False), ('parsed', True), ('stats […]*

```diff
@@ -57724,14 +57724,867 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 36
                 },
                 "empty": 0
             }
         },
+        "525": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "fastener 1",
+                            "elapsed": [
+                                0.03455425500214915,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "modules/fasten/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.204400152550079e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "insure/status_equalitites_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.051308581001649,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "flow/demux_mux/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.027234834000410046,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "flow/demux_mux2/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "runs without exceptions",
+                            "elapsed": [
+                                0.007963182997627882,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/files/scan/JSON/status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.15334440699734841,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/directory/equalize/_status/2/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.26066640699718846,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/directory/equalize/_status/1/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "EQ check with differences",
+                            "elapsed": [
+                                0.0007407260018226225,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/directory/check_equality/_status/2/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "EQ check without differences",
+                            "elapsed": [
+                                0.0005701750014850404,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/directory/check_equality/_status/1/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.23241425700325635,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/directory/scan_tree/_status/2/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.14625594700191868,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/directory/scan_tree/_status/1/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "runs without exceptions",
+                            "elapsed": [
+                                0.0036997659990447573,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/directory/find_and_replace_string_v2/_status/1.contents/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "runs without exceptions",
+                            "elapsed": [
+                                0.04754730300192023,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/directory/find_and_replace_string_v2/_status/2.contents/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "runs without exceptions",
+                            "elapsed": [
+                                0.15605596500245156,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "runs without exceptions",
+                            "elapsed": [
+                                0.007864855000661919,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/directory/find_and_replace_string/_status/1.contents/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "runs without exceptions",
+                            "elapsed": [
+                                0.00993590299913194,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/directory/find_and_replace_string/_status/2.contents/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0275290200006566,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/directory/size/_status/1/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0004404780011100229,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/directory/sense/_status/1/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.9078884720001952,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "process/start/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.0342743050023273,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "process/start/_status/2/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.778598383996723,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "process/multi_2/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.0837026439985493,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "process/multi_2/_status/2/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                8.520000847056508e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "process/multi/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.675283579999814,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "process/multi/_status/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.261592948998441,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "cycle/loops/status_4.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.251546409999719,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "cycle/loops/status_3.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.2696125029979157,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "cycle/loops/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.0018041269977402,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "cycle/params/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.002182031999837,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "cycle/params/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.0013281640021887,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "cycle/params_2/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.11051167699770303,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "cadence/filter/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.0921332249999978,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "cadence/filter/_status/status_3.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.0717696389983757,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "cadence/filter/_status/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.00011796400212915614,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "cadence/UTC/status_current.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "1",
+                            "elapsed": [
+                                0.4858736999995017,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "ports/find_multiple/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "1",
+                            "elapsed": [
+                                0.07700035399830085,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "ports/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 36
+                },
+                "empty": 0
+            }
+        },
+        "526": {
+            "alarms": [
+                {
+                    "alarm": "An exception occurred while importing the path.",
+                    "exception": "ImportError(\"cannot import name 'simultaneously_v2' from 'ships.flow.simultaneous_v2' (/ships/fields/gardens/ships/flow/simultaneous_v2/__init__.py)\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/ships/fields/gardens_pip/biotech/procedures/health_scan/process/modules/__import_from_path/__init__.py\", line 43, in import_from_path",
+                        "    proceeds = spec.loader.exec_module (the_module)",
+                        "  File \"<frozen importlib._bootstrap_external>\", line 883, in exec_module",
+                        "  File \"<frozen importlib._bootstrap>\", line 241, in _call_with_frames_removed",
+                        "  File \"/ships/fields/gardens/ships/flow/simultaneous_v2/_status/status_1.py\", line 14, in <module>",
+                        "    from ships.flow.simultaneous_v2 import simultaneously_v2",
+                        "ImportError: cannot import name 'simultaneously_v2' from 'ships.flow.simultaneous_v2' (/ships/fields/gardens/ships/flow/simultaneous_v2/__init__.py)"
+                    ],
+                    "parsed": false,
+                    "path": "flow/simultaneous_v2/_status/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "alarm": "An exception occurred while importing the path.",
+                    "exception": "ImportError(\"cannot import name 'simultaneously_v2' from 'ships.flow.simultaneous_v2' (/ships/fields/gardens/ships/flow/simultaneous_v2/__init__.py)\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/ships/fields/gardens_pip/biotech/procedures/health_scan/process/modules/__import_from_path/__init__.py\", line 43, in import_from_path",
+                        "    proceeds = spec.loader.exec_module (the_module)",
+                        "  File \"<frozen importlib._bootstrap_external>\", line 883, in exec_module",
+                        "  File \"<frozen importlib._bootstrap>\", line 241, in _call_with_frames_removed",
+                        "  File \"/ships/fields/gardens/ships/flow/simultaneous_v2/_status/status_1.py\", line 14, in <module>",
+                        "    from ships.flow.simultaneous_v2 import simultaneously_v2",
+                        "ImportError: cannot import name 'simultaneously_v2' from 'ships.flow.simultaneous_v2' (/ships/fields/gardens/ships/flow/simultaneous_v2/__init__.py)"
+                    ],
+                    "parsed": false,
+                    "path": "flow/simultaneous_v2/_status/status_1.py"
+                }
+            ],
+            "stats": {
+                "alarms": 1,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 0
+                },
+                "empty": 0
+            }
+        },
+        "527": {
+            "alarms": [
+                {
+                    "alarm": "An exception occurred while importing the path.",
+                    "exception": "ImportError(\"cannot import name 'simultaneously_v2' from 'ships.flow.simultaneous_v2' (/ships/fields/gardens/ships/flow/simultaneous_v2/__init__.py)\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/ships/fields/gardens_pip/biotech/procedures/health_scan/process/modules/__import_from_path/__init__.py\", line 43, in import_from_path",
+                        "    proceeds = spec.loader.exec_module (the_module)",
+                        "  File \"<frozen importlib._bootstrap_external>\", line 883, in exec_module",
+                        "  File \"<frozen importlib._bootstrap>\", line 241, in _call_with_frames_removed",
+                        "  File \"/ships/fields/gardens/ships/flow/simultaneous_v2/_status/status_1.py\", line 14, in <module>",
+                        "    from ships.flow.simultaneous_v2 import simultaneously_v2",
+                        "ImportError: cannot import name 'simultaneously_v2' from 'ships.flow.simultaneous_v2' (/ships/fields/gardens/ships/flow/simultaneous_v2/__init__.py)"
+                    ],
+                    "parsed": false,
+                    "path": "flow/simultaneous_v2/_status/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "alarm": "An exception occurred while importing the path.",
+                    "exception": "ImportError(\"cannot import name 'simultaneously_v2' from 'ships.flow.simultaneous_v2' (/ships/fields/gardens/ships/flow/simultaneous_v2/__init__.py)\")",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/ships/fields/gardens_pip/biotech/procedures/health_scan/process/modules/__import_from_path/__init__.py\", line 43, in import_from_path",
+                        "    proceeds = spec.loader.exec_module (the_module)",
+                        "  File \"<frozen importlib._bootstrap_external>\", line 883, in exec_module",
+                        "  File \"<frozen importlib._bootstrap>\", line 241, in _call_with_frames_removed",
+                        "  File \"/ships/fields/gardens/ships/flow/simultaneous_v2/_status/status_1.py\", line 14, in <module>",
+                        "    from ships.flow.simultaneous_v2 import simultaneously_v2",
+                        "ImportError: cannot import name 'simultaneously_v2' from 'ships.flow.simultaneous_v2' (/ships/fields/gardens/ships/flow/simultaneous_v2/__init__.py)"
+                    ],
+                    "parsed": false,
+                    "path": "flow/simultaneous_v2/_status/status_1.py"
+                }
+            ],
+            "stats": {
+                "alarms": 1,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 0
+                },
+                "empty": 0
+            }
+        },
+        "528": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.001487801993789617,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "flow/simultaneous_v2/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 1
+                },
+                "empty": 0
+            }
+        },
+        "529": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0015226579998852685,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "flow/simultaneous_v2/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 1
+                },
+                "empty": 0
+            }
+        },
         "53": {
             "alarms": [
                 {
                     "checks": [
                         {
                             "check": "check 1",
                             "exception": "KeyError('directories')",
@@ -57784,14 +58637,358 @@
                 "checks": {
                     "alarms": 1,
                     "passes": 0
                 },
                 "empty": 0
             }
         },
+        "530": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0014774689989280887,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "flow/simultaneous_v2/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 1
+                },
+                "empty": 0
+            }
+        },
+        "531": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "TypeError('list indices must be integers or slices, not str')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/ships/fields/gardens_pip/biotech/procedures/health_scan/process/modules/__import_from_path/__init__.py\", line 54, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/ships/fields/gardens/ships/flow/simultaneous_v2/_status/status_1.py\", line 54, in check_1",
+                                "    results = proceeds [\"results\"]",
+                                "TypeError: list indices must be integers or slices, not str"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "flow/simultaneous_v2/_status/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "TypeError('list indices must be integers or slices, not str')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/ships/fields/gardens_pip/biotech/procedures/health_scan/process/modules/__import_from_path/__init__.py\", line 54, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/ships/fields/gardens/ships/flow/simultaneous_v2/_status/status_1.py\", line 54, in check_1",
+                                "    results = proceeds [\"results\"]",
+                                "TypeError: list indices must be integers or slices, not str"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "flow/simultaneous_v2/_status/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 1,
+                    "passes": 0
+                },
+                "empty": 0
+            }
+        },
+        "532": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0020887940045213327,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "flow/simultaneous_v2/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 1
+                },
+                "empty": 0
+            }
+        },
+        "533": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0017174609965877607,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "flow/simultaneous_v2/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 1
+                },
+                "empty": 0
+            }
+        },
+        "534": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0010603720002109185,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "flow/simultaneous_v2/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 1
+                },
+                "empty": 0
+            }
+        },
+        "535": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0011809339994215406,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "flow/simultaneous_v2/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 1
+                },
+                "empty": 0
+            }
+        },
+        "536": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0011655790003715083,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "flow/simultaneous_v2/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 1
+                },
+                "empty": 0
+            }
+        },
+        "537": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.001186642999527976,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "flow/simultaneous_v2/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 1
+                },
+                "empty": 0
+            }
+        },
+        "538": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.04013351000321563,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "flow/simultaneous_v2/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 1
+                },
+                "empty": 0
+            }
+        },
+        "539": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.0385912530036876,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "flow/simultaneous_v2/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 1
+                },
+                "empty": 0
+            }
+        },
         "54": {
             "alarms": [
                 {
                     "checks": [
                         {
                             "check": "check 1",
                             "exception": "AttributeError(\"module 'botany.paths.directory.rsync' has no attribute 'process'\")",
@@ -57844,14 +59041,1110 @@
                 "checks": {
                     "alarms": 1,
                     "passes": 0
                 },
                 "empty": 0
             }
         },
+        "540": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.04320918600569712,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "flow/simultaneous_v2/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 1
+                },
+                "empty": 0
+            }
+        },
+        "541": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.03833177300111856,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "flow/simultaneous_v2/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 1
+                },
+                "empty": 0
+            }
+        },
+        "542": {
+            "alarms": [
+                {
+                    "alarm": "An exception occurred while importing the path.",
+                    "exception": "SyntaxError(\"invalid syntax. Maybe you meant '==' or ':=' instead of '='?\", ('/ships/fields/gardens/ships/flow/simultaneous_v2/_status/status_1.py', 64, 10, '\\tassert (anomalies = [ 1 ])\\n', 64, 27))",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/ships/fields/gardens_pip/biotech/procedures/health_scan/process/modules/__import_from_path/__init__.py\", line 43, in import_from_path",
+                        "    proceeds = spec.loader.exec_module (the_module)",
+                        "  File \"<frozen importlib._bootstrap_external>\", line 879, in exec_module",
+                        "  File \"<frozen importlib._bootstrap_external>\", line 1017, in get_code",
+                        "  File \"<frozen importlib._bootstrap_external>\", line 947, in source_to_code",
+                        "  File \"<frozen importlib._bootstrap>\", line 241, in _call_with_frames_removed",
+                        "  File \"/ships/fields/gardens/ships/flow/simultaneous_v2/_status/status_1.py\", line 64",
+                        "    \tassert (anomalies = [ 1 ])",
+                        "    \t        ^^^^^^^^^^^^^^^^^",
+                        "SyntaxError: invalid syntax. Maybe you meant '==' or ':=' instead of '='?"
+                    ],
+                    "parsed": false,
+                    "path": "flow/simultaneous_v2/_status/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "alarm": "An exception occurred while importing the path.",
+                    "exception": "SyntaxError(\"invalid syntax. Maybe you meant '==' or ':=' instead of '='?\", ('/ships/fields/gardens/ships/flow/simultaneous_v2/_status/status_1.py', 64, 10, '\\tassert (anomalies = [ 1 ])\\n', 64, 27))",
+                    "exception trace": [
+                        "Traceback (most recent call last):",
+                        "  File \"/ships/fields/gardens_pip/biotech/procedures/health_scan/process/modules/__import_from_path/__init__.py\", line 43, in import_from_path",
+                        "    proceeds = spec.loader.exec_module (the_module)",
+                        "  File \"<frozen importlib._bootstrap_external>\", line 879, in exec_module",
+                        "  File \"<frozen importlib._bootstrap_external>\", line 1017, in get_code",
+                        "  File \"<frozen importlib._bootstrap_external>\", line 947, in source_to_code",
+                        "  File \"<frozen importlib._bootstrap>\", line 241, in _call_with_frames_removed",
+                        "  File \"/ships/fields/gardens/ships/flow/simultaneous_v2/_status/status_1.py\", line 64",
+                        "    \tassert (anomalies = [ 1 ])",
+                        "    \t        ^^^^^^^^^^^^^^^^^",
+                        "SyntaxError: invalid syntax. Maybe you meant '==' or ':=' instead of '='?"
+                    ],
+                    "parsed": false,
+                    "path": "flow/simultaneous_v2/_status/status_1.py"
+                }
+            ],
+            "stats": {
+                "alarms": 1,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 0
+                },
+                "empty": 0
+            }
+        },
+        "543": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError()",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/ships/fields/gardens_pip/biotech/procedures/health_scan/process/modules/__import_from_path/__init__.py\", line 54, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/ships/fields/gardens/ships/flow/simultaneous_v2/_status/status_1.py\", line 69, in check_1",
+                                "    assert (results [index] == items [index] + 1)",
+                                "AssertionError"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "flow/simultaneous_v2/_status/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError()",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/ships/fields/gardens_pip/biotech/procedures/health_scan/process/modules/__import_from_path/__init__.py\", line 54, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/ships/fields/gardens/ships/flow/simultaneous_v2/_status/status_1.py\", line 69, in check_1",
+                                "    assert (results [index] == items [index] + 1)",
+                                "AssertionError"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "flow/simultaneous_v2/_status/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 1,
+                    "passes": 0
+                },
+                "empty": 0
+            }
+        },
+        "544": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError([0])",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/ships/fields/gardens_pip/biotech/procedures/health_scan/process/modules/__import_from_path/__init__.py\", line 54, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/ships/fields/gardens/ships/flow/simultaneous_v2/_status/status_1.py\", line 69, in check_1",
+                                "    assert (results [index] == items [index] + 1), [ index ]",
+                                "AssertionError: [0]"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "flow/simultaneous_v2/_status/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError([0])",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/ships/fields/gardens_pip/biotech/procedures/health_scan/process/modules/__import_from_path/__init__.py\", line 54, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/ships/fields/gardens/ships/flow/simultaneous_v2/_status/status_1.py\", line 69, in check_1",
+                                "    assert (results [index] == items [index] + 1), [ index ]",
+                                "AssertionError: [0]"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "flow/simultaneous_v2/_status/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 1,
+                    "passes": 0
+                },
+                "empty": 0
+            }
+        },
+        "545": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError([0, {'result': 4.5, 'anomaly': 'no', 'exception': ''}, 3.5])",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/ships/fields/gardens_pip/biotech/procedures/health_scan/process/modules/__import_from_path/__init__.py\", line 54, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/ships/fields/gardens/ships/flow/simultaneous_v2/_status/status_1.py\", line 69, in check_1",
+                                "    assert (results [index] == items [index] + 1), [",
+                                "AssertionError: [0, {'result': 4.5, 'anomaly': 'no', 'exception': ''}, 3.5]"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "flow/simultaneous_v2/_status/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "exception": "AssertionError([0, {'result': 4.5, 'anomaly': 'no', 'exception': ''}, 3.5])",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/ships/fields/gardens_pip/biotech/procedures/health_scan/process/modules/__import_from_path/__init__.py\", line 54, in import_from_path",
+                                "    checks [ check ] ()",
+                                "  File \"/ships/fields/gardens/ships/flow/simultaneous_v2/_status/status_1.py\", line 69, in check_1",
+                                "    assert (results [index] == items [index] + 1), [",
+                                "AssertionError: [0, {'result': 4.5, 'anomaly': 'no', 'exception': ''}, 3.5]"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "flow/simultaneous_v2/_status/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 1,
+                    "passes": 0
+                },
+                "empty": 0
+            }
+        },
+        "546": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.04131296400009887,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "flow/simultaneous_v2/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 1
+                },
+                "empty": 0
+            }
+        },
+        "547": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.04320335000375053,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "flow/simultaneous_v2/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 1
+                },
+                "empty": 0
+            }
+        },
+        "548": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.038896848003787454,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "flow/simultaneous_v2/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 1
+                },
+                "empty": 0
+            }
+        },
+        "549": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "fastener 1",
+                            "elapsed": [
+                                0.014225323000573553,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "modules/fasten/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.2947999241296202e-05,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "insure/status_equalitites_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.0074503970026853,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "flow/demux_mux/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.4055402630037861,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "flow/simultaneous_v2/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.053904984997643624,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "flow/demux_mux2/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "runs without exceptions",
+                            "elapsed": [
+                                0.00036471599742071703,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/files/scan/JSON/status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.3226254719993449,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/directory/equalize/_status/2/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.32866501799435355,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/directory/equalize/_status/1/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "EQ check with differences",
+                            "elapsed": [
+                                0.020765348999702837,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/directory/check_equality/_status/2/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "EQ check without differences",
+                            "elapsed": [
+                                0.0004883989968220703,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/directory/check_equality/_status/1/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.08818483299546642,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/directory/scan_tree/_status/2/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.13360357900091913,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/directory/scan_tree/_status/1/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "runs without exceptions",
+                            "elapsed": [
+                                0.0031984279994503595,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/directory/find_and_replace_string_v2/_status/1.contents/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "runs without exceptions",
+                            "elapsed": [
+                                0.004923938002320938,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/directory/find_and_replace_string_v2/_status/2.contents/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "runs without exceptions",
+                            "elapsed": [
+                                0.09214523200353142,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "runs without exceptions",
+                            "elapsed": [
+                                0.002860661996237468,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/directory/find_and_replace_string/_status/1.contents/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "runs without exceptions",
+                            "elapsed": [
+                                0.0028654400011873804,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/directory/find_and_replace_string/_status/2.contents/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.03537361000053352,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/directory/size/_status/1/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.00046756699885008857,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "paths/directory/sense/_status/1/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.7364270010002656,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "process/start/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.040535177999118,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "process/start/_status/2/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.8104966660030186,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "process/multi_2/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.03347577599925,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "process/multi_2/_status/2/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                8.049973985180259e-07,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "process/multi/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.6038677239994286,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "process/multi/_status/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.2530433389983955,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "cycle/loops/status_4.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.2517112249988713,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "cycle/loops/status_3.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.2555660380021436,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "cycle/loops/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.0018230990026495,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "cycle/params/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.002089840003464,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "cycle/params/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.001059513000655,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "cycle/params_2/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.10932646400033263,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "cadence/filter/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.0637284189942875,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "cadence/filter/_status/status_3.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.087632315000519,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "cadence/filter/_status/status_2.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                0.00025911299599101767,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "cadence/UTC/status_current.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "1",
+                            "elapsed": [
+                                0.2602561129970127,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "ports/find_multiple/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "1",
+                            "elapsed": [
+                                0.12503186999674654,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "ports/_status/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 37
+                },
+                "empty": 0
+            }
+        },
         "55": {
             "alarms": [
                 {
                     "checks": [
                         {
                             "check": "check 1",
                             "exception": "NameError(\"name 'REPORT' is not defined\")",
```

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/coverage_html.js` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/coverage_html.js`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_45774dabac2a4451___init___py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_45774dabac2a4451___init___py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad___init___py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad___init___py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__cell_widths_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__cell_widths_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__emoji_codes_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__emoji_codes_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__emoji_replace_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__emoji_replace_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__export_format_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__export_format_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__fileno_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__fileno_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__log_render_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__log_render_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__loop_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__loop_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__null_file_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__null_file_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__palettes_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__palettes_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__pick_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__pick_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__ratio_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__ratio_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__wrap_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad__wrap_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_abc_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_abc_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_align_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_align_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_box_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_box_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_cells_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_cells_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_color_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_color_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_color_triplet_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_color_triplet_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_console_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_console_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_constrain_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_constrain_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_containers_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_containers_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_control_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_control_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_default_styles_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_default_styles_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_emoji_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_emoji_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_errors_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_errors_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_highlighter_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_highlighter_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_json_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_json_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_jupyter_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_jupyter_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_markup_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_markup_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_measure_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_measure_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_padding_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_padding_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_pager_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_pager_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_palette_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_palette_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_panel_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_panel_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_pretty_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_pretty_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_protocol_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_protocol_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_region_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_region_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_repr_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_repr_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_scope_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_scope_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_screen_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_screen_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_segment_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_segment_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_style_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_style_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_styled_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_styled_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_table_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_table_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_terminal_theme_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_terminal_theme_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_text_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_text_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_theme_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_theme_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_themes_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_94f2f3fde87e2bad_themes_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_9c84d462c231d294_exceptions_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_9c84d462c231d294_exceptions_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_9c84d462c231d294_expect_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_9c84d462c231d294_expect_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_9c84d462c231d294_pty_spawn_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_9c84d462c231d294_pty_spawn_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_9c84d462c231d294_spawnbase_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_9c84d462c231d294_spawnbase_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_9c84d462c231d294_utils_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_9c84d462c231d294_utils_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_acd758f7e5b0fd78_ptyprocess_py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_acd758f7e5b0fd78_ptyprocess_py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/d_f85661004356945c___init___py.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/d_f85661004356945c___init___py.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/favicon_32.png` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/favicon_32.png`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/index.html` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/index.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/keybd_closed.png` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/keybd_open.png` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/keybd_open.png`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/status.json` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/status.json`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/coverage_report/style.css` & `ships-1.3.8/fields/gardens/ships/_status/coverage_report/style.css`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/_status/status.proc.py` & `ships-1.3.8/fields/gardens/ships/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/business/decorators/examples/example_1.py` & `ships-1.3.8/fields/gardens/ships/business/decorators/examples/example_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cadence/UTC/__pycache__/MONTH_STRINGS.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/cadence/UTC/__pycache__/MONTH_STRINGS.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cadence/UTC/__pycache__/NOW.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/cadence/UTC/__pycache__/NOW.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cadence/UTC/__pycache__/NOW.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/cadence/UTC/__pycache__/NOW.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cadence/UTC/__pycache__/current.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/cadence/UTC/__pycache__/current.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cadence/UTC/__pycache__/current.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/cadence/UTC/__pycache__/current.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cadence/UTC/__pycache__/now.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/cadence/UTC/__pycache__/now.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cadence/UTC/__pycache__/status_current.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/cadence/UTC/__pycache__/status_current.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cadence/UTC/__pycache__/test_NOW.cpython-310-pytest-7.4.0.pyc` & `ships-1.3.8/fields/gardens/ships/cadence/UTC/__pycache__/test_NOW.cpython-310-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cadence/UTC/__pycache__/test_NOW.cpython-311-pytest-7.4.0.pyc` & `ships-1.3.8/fields/gardens/ships/cadence/UTC/__pycache__/test_NOW.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cadence/UTC/current.py` & `ships-1.3.8/fields/gardens/ships/cadence/UTC/current.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cadence/UTC/month/__pycache__/strings.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/cadence/UTC/month/__pycache__/strings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cadence/UTC/month/__pycache__/strings.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/cadence/UTC/month/__pycache__/strings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cadence/UTC/status_current.py` & `ships-1.3.8/fields/gardens/ships/cadence/UTC/status_current.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cadence/filter/__init__.py` & `ships-1.3.8/fields/gardens/ships/cadence/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cadence/filter/__pycache__/__init__.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/cadence/filter/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cadence/filter/__pycache__/__init__.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/cadence/filter/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cadence/filter/_status/__pycache__/status_1.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/cadence/filter/_status/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cadence/filter/_status/__pycache__/status_2.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/cadence/filter/_status/__pycache__/status_2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cadence/filter/_status/__pycache__/status_3.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/cadence/filter/_status/__pycache__/status_3.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cadence/filter/_status/status_1.py` & `ships-1.3.8/fields/gardens/ships/cadence/filter/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cadence/filter/_status/status_2.py` & `ships-1.3.8/fields/gardens/ships/cadence/filter/_status/status_2.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cadence/filter/_status/status_3.py` & `ships-1.3.8/fields/gardens/ships/cadence/filter/_status/status_3.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/coms/protocols/SSH/SSH.r.HTML` & `ships-1.3.8/fields/gardens/ships/coms/protocols/SSH/SSH.r.HTML`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/__pycache__/__init__.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/cycle/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/__pycache__/loops.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/cycle/__pycache__/loops.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/__pycache__/params.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/cycle/__pycache__/params.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/__pycache__/presents.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/cycle/__pycache__/presents.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/cycle.S.HTML` & `ships-1.3.8/fields/gardens/ships/cycle/cycle.S.HTML`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/loops/__init__.py` & `ships-1.3.8/fields/gardens/ships/cycle/loops/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/loops/__pycache__/__init__.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/cycle/loops/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/loops/__pycache__/__init__.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/cycle/loops/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/loops/__pycache__/status_2.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/cycle/loops/__pycache__/status_2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/loops/__pycache__/status_3.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/cycle/loops/__pycache__/status_3.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/loops/__pycache__/status_4.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/cycle/loops/__pycache__/status_4.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/loops/status_2.py` & `ships-1.3.8/fields/gardens/ships/cycle/loops/status_2.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/loops/status_3.py` & `ships-1.3.8/fields/gardens/ships/cycle/loops/status_3.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/loops/status_4.py` & `ships-1.3.8/fields/gardens/ships/cycle/loops/status_4.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/params/__init__.py` & `ships-1.3.8/fields/gardens/ships/cycle/params/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/params/__pycache__/__init__.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/cycle/params/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/params/__pycache__/__init__.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/cycle/params/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/params/__pycache__/status_1.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/cycle/params/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/params/__pycache__/status_2.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/cycle/params/__pycache__/status_2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/params/status_2.py` & `ships-1.3.8/fields/gardens/ships/cycle/params/status_2.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/params_2/__init__.py` & `ships-1.3.8/fields/gardens/ships/cycle/params_2/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/params_2/__pycache__/__init__.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/cycle/params_2/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/params_2/__pycache__/__init__.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/cycle/params_2/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/params_2/__pycache__/status_1.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/cycle/params_2/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/params_2/status_1.py` & `ships-1.3.8/fields/gardens/ships/cycle/params_2/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/presents/__pycache__/__init__.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/cycle/presents/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/cycle/presents/__pycache__/__init__.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/cycle/presents/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/flow/demux_mux/__init__.py` & `ships-1.3.8/fields/gardens/ships/flow/demux_mux/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/flow/demux_mux/__pycache__/__init__.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/flow/demux_mux/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/flow/demux_mux/__pycache__/__init__.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/flow/demux_mux/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/flow/demux_mux/_status/__pycache__/status_1.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/flow/demux_mux/_status/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/flow/demux_mux/_status/status_1.py` & `ships-1.3.8/fields/gardens/ships/flow/demux_mux/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/flow/demux_mux2/__init__.py` & `ships-1.3.8/fields/gardens/ships/flow/demux_mux2/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/flow/demux_mux2/__pycache__/__init__.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/flow/demux_mux2/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/flow/demux_mux2/__pycache__/__init__.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/flow/demux_mux2/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/flow/demux_mux2/_status/__pycache__/status_1.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/flow/demux_mux2/_status/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/flow/demux_mux2/_status/status_1.py` & `ships-1.3.8/fields/gardens/ships/flow/demux_mux2/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/flow/simultaneous/__init__.py` & `ships-1.3.8/fields/gardens/ships/flow/simultaneous/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,30 +38,34 @@
 	#
 	semaphore = threading.Semaphore (capacity)
 
 	# Define a function to process items with semaphore limit and return results
 	def process_with_semaphore (item, index, results_queue):
 		with semaphore:
 			result = move (item)
-			results_queue.put((index, result))  # Put the result along with its index in the queue
+			results_queue.put ((index, result))  # Put the result along with its index in the queue
 
 	# Create a queue to collect the results
 	results_queue = Queue ()
 
 	# Create threads to process items
 	threads = []
 	for index, item in enumerate (items):
-		thread = threading.Thread (target=process_with_semaphore, args=(item, index, results_queue))
-		thread.start()
-		threads.append(thread)
+		thread = threading.Thread (
+			target = process_with_semaphore, 
+			args = (item, index, results_queue)
+		)
+		
+		thread.start ()
+		threads.append (thread)
 
 	# Wait for all threads to complete
 	for thread in threads:
-		thread.join()
+		thread.join ()
 
 	# Collect results from the queue and reorder them based on the original item order
-	results = [None] * len(items)
-	while not results_queue.empty():
-		index, result = results_queue.get()
-		results[index] = result
+	results = [None] * len (items)
+	while not results_queue.empty ():
+		index, result = results_queue.get ()
+		results [index] = result
 	
 	return results;
```

### Comparing `ships-1.2.8/fields/gardens/ships/formats/ISO/ISO.s.HTML` & `ships-1.3.8/fields/gardens/ships/formats/ISO/ISO.s.HTML`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/glamour/UTF8/one.HTML` & `ships-1.3.8/fields/gardens/ships/glamour/UTF8/one.HTML`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/insure/__pycache__/equalities.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/insure/__pycache__/equalities.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/insure/__pycache__/equalities.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/insure/__pycache__/equalities.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/insure/__pycache__/equality.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/insure/__pycache__/equality.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/insure/__pycache__/status_equalitites_1.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/insure/__pycache__/status_equalitites_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/insure/equalities.py` & `ships-1.3.8/fields/gardens/ships/insure/equalities.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/module.MD` & `ships-1.3.8/fields/gardens/ships/module.MD`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/modules/exceptions/__pycache__/parse.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/modules/exceptions/__pycache__/parse.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/modules/exceptions/__pycache__/parse.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/modules/exceptions/__pycache__/parse.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/modules/fasten/__init__.py` & `ships-1.3.8/fields/gardens/ships/modules/fasten/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/modules/fasten/__pycache__/__init__.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/modules/fasten/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/modules/fasten/__pycache__/__init__.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/modules/fasten/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/modules/fasten/_status/__pycache__/example_caller.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/modules/fasten/_status/__pycache__/example_caller.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/modules/fasten/_status/__pycache__/status_1.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/modules/fasten/_status/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/modules/print/print.s.HTML` & `ships-1.3.8/fields/gardens/ships/modules/print/print.s.HTML`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/__init__.py` & `ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/__pycache__/__init__.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/__pycache__/__init__.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/_status/1/__pycache__/status_1.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/_status/1/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/_status/1/status_1.py` & `ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/_status/1/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/_status/2/__pycache__/status_1.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/_status/2/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/_status/2/status_1.py` & `ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/_status/2/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/ADD_DIFFERENT_CONTENTS.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/ADD_DIFFERENT_CONTENTS.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/ADD_DIFFERENT_PATHS.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/ADD_DIFFERENT_PATHS.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/GET_DIRECTORIES.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/GET_DIRECTORIES.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/GET_SAME_DIRECTORIES.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/GET_SAME_DIRECTORIES.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/add_different_contents.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/add_different_contents.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/add_different_contents.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/add_different_contents.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/add_different_paths.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/add_different_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/add_different_paths.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/add_different_paths.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/get_directories.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/get_directories.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/get_directories.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/get_directories.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/get_same_directories.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/get_same_directories.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/get_same_directories.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/__pycache__/get_same_directories.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/add_different_contents.py` & `ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/add_different_contents.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/check_equality/courses/add_different_paths.py` & `ships-1.3.8/fields/gardens/ships/paths/directory/check_equality/courses/add_different_paths.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/deallocate/__pycache__/__init__.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/deallocate/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/equalize/__init__.py` & `ships-1.3.8/fields/gardens/ships/paths/directory/equalize/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/equalize/__pycache__/__init__.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/equalize/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/equalize/__pycache__/__init__.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/equalize/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/equalize/_status/1/__pycache__/status_1.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/equalize/_status/1/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/equalize/_status/1/status_1.py` & `ships-1.3.8/fields/gardens/ships/paths/directory/equalize/_status/1/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/equalize/_status/2/__pycache__/status_1.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/equalize/_status/2/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/equalize/_status/2/status_1.py` & `ships-1.3.8/fields/gardens/ships/paths/directory/equalize/_status/2/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/__init__.py` & `ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/__pycache__/__init__.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/__pycache__/__init__.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/1.contents/__pycache__/status_1.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/1.contents/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/1.contents/status_1.py` & `ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/1.contents/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/2.contents/__pycache__/status_1.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/2.contents/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/2.contents/status_1.py` & `ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string/_status/2.contents/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/__init__.py` & `ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/__pycache__/__init__.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/__pycache__/__init__.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/1.contents/__pycache__/status_1.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/1.contents/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/1.contents/status_1.py` & `ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/1.contents/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/2.contents/__pycache__/status_1.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/2.contents/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/2.contents/status_1.py` & `ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/2.contents/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/__pycache__/status_1.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/status_1.py` & `ships-1.3.8/fields/gardens/ships/paths/directory/find_and_replace_string_v2/_status/3.contents_and_paths/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/for_each_path/__init__.py` & `ships-1.3.8/fields/gardens/ships/paths/directory/for_each_path/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/rsync/__init__.py` & `ships-1.3.8/fields/gardens/ships/paths/directory/rsync/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/rsync/__pycache__/__init__.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/rsync/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/rsync/__pycache__/__init__.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/rsync/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/scan_tree/DFS.py` & `ships-1.3.8/fields/gardens/ships/paths/directory/scan_tree/DFS.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/scan_tree/__init__.py` & `ships-1.3.8/fields/gardens/ships/paths/directory/scan_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/scan_tree/__init__v1.py` & `ships-1.3.8/fields/gardens/ships/paths/directory/scan_tree/__init__v1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/scan_tree/__pycache__/DFS.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/scan_tree/__pycache__/DFS.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/scan_tree/__pycache__/__init__.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/scan_tree/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/scan_tree/_status/1/__pycache__/status_1.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/scan_tree/_status/1/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/scan_tree/_status/1/status_1.py` & `ships-1.3.8/fields/gardens/ships/paths/directory/scan_tree/_status/1/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/scan_tree/_status/2/__pycache__/status_1.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/scan_tree/_status/2/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/scan_tree/_status/2/status_1.py` & `ships-1.3.8/fields/gardens/ships/paths/directory/scan_tree/_status/2/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/sense/__init__.py` & `ships-1.3.8/fields/gardens/ships/paths/directory/sense/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/sense/__pycache__/__init__.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/sense/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/sense/__pycache__/__init__.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/sense/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/sense/_status/1/__pycache__/status_1.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/sense/_status/1/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/sense/_status/1/status_1.py` & `ships-1.3.8/fields/gardens/ships/paths/directory/sense/_status/1/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/size/__init__.py` & `ships-1.3.8/fields/gardens/ships/paths/directory/size/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/size/__pycache__/__init__.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/size/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/size/__pycache__/__init__.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/size/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/size/_status/1/__pycache__/status_1.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/directory/size/_status/1/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/directory/size/_status/1/status_1.py` & `ships-1.3.8/fields/gardens/ships/paths/directory/size/_status/1/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/files/scan/JSON/__init__.py` & `ships-1.3.8/fields/gardens/ships/paths/files/scan/JSON/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/files/scan/JSON/__pycache__/JSON.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/paths/files/scan/JSON/__pycache__/JSON.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/files/scan/JSON/__pycache__/__init__.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/files/scan/JSON/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/files/scan/JSON/__pycache__/__init__.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/paths/files/scan/JSON/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/files/scan/JSON/status/__pycache__/status_1.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/paths/files/scan/JSON/status/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/files/scan/JSON/status/status_1.py` & `ships-1.3.8/fields/gardens/ships/paths/files/scan/JSON/status/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/fs, rsync details.r.html` & `ships-1.3.8/fields/gardens/ships/paths/fs, rsync details.r.html`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/paths/path/__pycache__/relative.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/paths/path/__pycache__/relative.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/ANSI.py` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/ANSI.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/FSM.py` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/FSM.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__init__.py` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/ANSI.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/ANSI.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/FSM.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/FSM.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/__init__.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/__init__.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/_async.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/_async.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/_async_pre_await.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/_async_pre_await.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/_async_w_await.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/_async_w_await.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/exceptions.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/exceptions.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/expect.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/expect.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/expect.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/expect.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/fdpexpect.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/fdpexpect.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/popen_spawn.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/popen_spawn.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/pty_spawn.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/pty_spawn.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/pty_spawn.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/pty_spawn.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/pxssh.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/pxssh.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/replwrap.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/replwrap.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/run.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/run.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/run.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/run.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/screen.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/screen.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/socket_pexpect.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/socket_pexpect.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/spawnbase.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/spawnbase.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/spawnbase.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/spawnbase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/utils.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/utils.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/_async.py` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/_async.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/_async_pre_await.py` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/_async_pre_await.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/_async_w_await.py` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/_async_w_await.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/exceptions.py` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/exceptions.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/expect.py` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/expect.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/fdpexpect.py` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/fdpexpect.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/pexpect-4.9.0.dist-info/LICENSE` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/pexpect-4.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/pexpect-4.9.0.dist-info/METADATA` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/pexpect-4.9.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/pexpect-4.9.0.dist-info/RECORD` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/pexpect-4.9.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/popen_spawn.py` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/popen_spawn.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/pty_spawn.py` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/pty_spawn.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/pxssh.py` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/pxssh.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/replwrap.py` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/replwrap.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/run.py` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/run.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/screen.py` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/screen.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/socket_pexpect.py` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/socket_pexpect.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/spawnbase.py` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/spawnbase.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/pexpect_4_9_0_copy/utils.py` & `ships-1.3.8/fields/gardens/ships/pexpect_4_9_0_copy/utils.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/ports/__pycache__/available.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/ports/__pycache__/available.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/ports/__pycache__/available.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/ports/__pycache__/available.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/ports/__pycache__/claimed.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/ports/__pycache__/claimed.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/ports/__pycache__/claimed.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/ports/__pycache__/claimed.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/ports/_status/__pycache__/status_1.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/ports/_status/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/ports/available.py` & `ships-1.3.8/fields/gardens/ships/ports/available.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/ports/find_multiple/__init__.py` & `ships-1.3.8/fields/gardens/ships/ports/find_multiple/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/ports/find_multiple/__pycache__/__init__.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/ports/find_multiple/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/ports/find_multiple/__pycache__/__init__.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/ports/find_multiple/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/ports/find_multiple/__pycache__/status_1.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/ports/find_multiple/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/multi/__init__.py` & `ships-1.3.8/fields/gardens/ships/process/multi/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/multi/__pycache__/__init__.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/process/multi/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/multi/__pycache__/__init__.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/process/multi/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/multi/_status/__pycache__/status_1.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/process/multi/_status/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/multi/_status/__pycache__/status_2.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/process/multi/_status/__pycache__/status_2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/multi/_status/status_1.py` & `ships-1.3.8/fields/gardens/ships/process/multi/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/multi/_status/status_2.py` & `ships-1.3.8/fields/gardens/ships/process/multi/_status/status_2.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/multi_2/__init__.py` & `ships-1.3.8/fields/gardens/ships/process/multi_2/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/multi_2/__pycache__/__init__.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/process/multi_2/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/multi_2/__pycache__/__init__.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/process/multi_2/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/multi_2/_status/2/__pycache__/status_2.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/process/multi_2/_status/2/__pycache__/status_2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/multi_2/_status/2/status_2.py` & `ships-1.3.8/fields/gardens/ships/process/multi_2/_status/2/status_2.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/multi_2/_status/__pycache__/status_1.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/process/multi_2/_status/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/multi_2/_status/status_1.py` & `ships-1.3.8/fields/gardens/ships/process/multi_2/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/start/__init__.py` & `ships-1.3.8/fields/gardens/ships/process/start/__init__.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/start/__pycache__/__init__.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/process/start/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/start/__pycache__/__init__.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/process/start/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/start/_status/.coverage` & `ships-1.3.8/fields/gardens/ships/process/start/_status/.coverage`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/start/_status/.status_1_coverage` & `ships-1.3.8/fields/gardens/ships/process/start/_status/.status_1_coverage`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/start/_status/2/.coverage` & `ships-1.3.8/fields/gardens/ships/process/start/_status/2/.coverage`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/start/_status/2/__pycache__/status_2.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/process/start/_status/2/__pycache__/status_2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/start/_status/2/status_2.py` & `ships-1.3.8/fields/gardens/ships/process/start/_status/2/status_2.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/start/_status/__pycache__/status_1.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/process/start/_status/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/start/_status/status_1.py` & `ships-1.3.8/fields/gardens/ships/process/start/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/start/parts/__pycache__/awareness.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/process/start/parts/__pycache__/awareness.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/start/parts/__pycache__/awareness.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/process/start/parts/__pycache__/awareness.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/start/parts/__pycache__/returns.cpython-310.pyc` & `ships-1.3.8/fields/gardens/ships/process/start/parts/__pycache__/returns.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/start/parts/__pycache__/returns.cpython-311.pyc` & `ships-1.3.8/fields/gardens/ships/process/start/parts/__pycache__/returns.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/fields/gardens/ships/process/start/parts/awareness.py` & `ships-1.3.8/fields/gardens/ships/process/start/parts/awareness.py`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/pyproject.toml` & `ships-1.3.8/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "ships"
-version = "1.2.8"
+version = "1.3.8"
 description = "Various calculator tools"
 authors = []
 readme = "readme.md"
 
 packages = [
     { include = "ships", from = "fields/gardens" }
 ]
```

### Comparing `ships-1.2.8/readme.md` & `ships-1.3.8/readme.md`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/ships.S.HTML` & `ships-1.3.8/ships.S.HTML`

 * *Files identical despite different names*

### Comparing `ships-1.2.8/PKG-INFO` & `ships-1.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ships
-Version: 1.2.8
+Version: 1.3.8
 Summary: Various calculator tools
 License: GPL-3.0-only
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

