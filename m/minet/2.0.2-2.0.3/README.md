# Comparing `tmp/minet-2.0.2.tar.gz` & `tmp/minet-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minet-2.0.2.tar", last modified: Mon Apr 22 08:04:56 2024, max compression
+gzip compressed data, was "minet-2.0.3.tar", last modified: Wed Apr 24 08:33:03 2024, max compression
```

## Comparing `minet-2.0.2.tar` & `minet-2.0.3.tar`

### file list

```diff
@@ -1,312 +1,312 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.103664 minet-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-22 08:03:40.000000 minet-2.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-04-22 08:04:56.103664 minet-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-04-22 08:03:40.000000 minet-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.067664 minet-2.0.2/minet/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-22 08:03:40.000000 minet-2.0.2/minet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-22 08:03:40.000000 minet-2.0.2/minet/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.067664 minet-2.0.2/minet/browser/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-22 08:03:40.000000 minet-2.0.2/minet/browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-22 08:03:40.000000 minet-2.0.2/minet/browser/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-22 08:03:40.000000 minet-2.0.2/minet/browser/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-22 08:03:40.000000 minet-2.0.2/minet/browser/plawright_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)    11839 2024-04-22 08:03:40.000000 minet-2.0.2/minet/browser/threadsafe_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-22 08:03:40.000000 minet-2.0.2/minet/browser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.067664 minet-2.0.2/minet/buzzsumo/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-22 08:03:40.000000 minet-2.0.2/minet/buzzsumo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-22 08:03:40.000000 minet-2.0.2/minet/buzzsumo/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-22 08:03:40.000000 minet-2.0.2/minet/buzzsumo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-04-22 08:03:40.000000 minet-2.0.2/minet/buzzsumo/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.071664 minet-2.0.2/minet/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30498 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/argparse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.071664 minet-2.0.2/minet/cli/buzzsumo/
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/buzzsumo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/buzzsumo/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/buzzsumo/domain_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/buzzsumo/exact_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/buzzsumo/limit.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/buzzsumo/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/console.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.071664 minet-2.0.2/minet/cli/cookies/
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/cookies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/cookies/cookies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.071664 minet-2.0.2/minet/cli/crawl/
--rw-r--r--   0 runner    (1001) docker     (127)    14843 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/crawl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12602 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/crawl/crawl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/crawl/focus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.071664 minet-2.0.2/minet/cli/crowdtangle/
--rw-r--r--   0 runner    (1001) docker     (127)    11696 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/crowdtangle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/crowdtangle/leaderboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/crowdtangle/lists.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/crowdtangle/posts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/crowdtangle/posts_by_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/crowdtangle/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/crowdtangle/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/crowdtangle/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.071664 minet-2.0.2/minet/cli/dump/
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/dump/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/dump/dump_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/dump/dump_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/dump/dump_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.071664 minet-2.0.2/minet/cli/extract/
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/extract/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.075664 minet-2.0.2/minet/cli/facebook/
--rw-r--r--   0 runner    (1001) docker     (127)    10645 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/facebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/facebook/comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/facebook/experimental_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/facebook/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/facebook/post_authors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7355 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/facebook/post_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/facebook/posts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/facebook/url_likes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/facebook/user_infos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/facebook/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.075664 minet-2.0.2/minet/cli/fetch/
--rw-r--r--   0 runner    (1001) docker     (127)    14730 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/fetch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18311 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/fetch/fetch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.075664 minet-2.0.2/minet/cli/google/
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/google/sheets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.075664 minet-2.0.2/minet/cli/hyphe/
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/hyphe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/hyphe/crawl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/hyphe/declare.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/hyphe/destroy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/hyphe/dump.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/hyphe/reset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/hyphe/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/hyphe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.079664 minet-2.0.2/minet/cli/instagram/
--rw-r--r--   0 runner    (1001) docker     (127)    11067 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/instagram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/instagram/comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/instagram/hashtag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/instagram/post_infos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/instagram/user_followers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/instagram/user_following.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/instagram/user_infos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/instagram/user_posts.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/instagram/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15677 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/loading_bar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.079664 minet-2.0.2/minet/cli/mediacloud/
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/mediacloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/mediacloud/medias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/mediacloud/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.079664 minet-2.0.2/minet/cli/mediacloud/topic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/mediacloud/topic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/mediacloud/topic/stories.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/mediacloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/reporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.079664 minet-2.0.2/minet/cli/scrape/
--rw-r--r--   0 runner    (1001) docker     (127)     8280 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/scrape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/scrape/scrape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.079664 minet-2.0.2/minet/cli/telegram/
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/telegram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/telegram/channel_infos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/telegram/channel_messages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.079664 minet-2.0.2/minet/cli/tiktok/
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/tiktok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/tiktok/search_videos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.083664 minet-2.0.2/minet/cli/twitter/
--rw-r--r--   0 runner    (1001) docker     (127)    24913 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/twitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10869 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/twitter/attrition.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/twitter/followers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/twitter/followers_you_know.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/twitter/friends.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/twitter/legacy_tweets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/twitter/list_followers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/twitter/list_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/twitter/retweeters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/twitter/scrape.py
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/twitter/tweet_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/twitter/tweet_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/twitter/tweet_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/twitter/tweets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/twitter/user_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/twitter/user_tweets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/twitter/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     8182 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/twitter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.083664 minet-2.0.2/minet/cli/url_extract/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/url_extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/url_extract/url_extract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.083664 minet-2.0.2/minet/cli/url_join/
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/url_join/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/url_join/url_join.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.083664 minet-2.0.2/minet/cli/url_parse/
--rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/url_parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/url_parse/url_parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.083664 minet-2.0.2/minet/cli/user_agents/
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/user_agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/user_agents/export.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/user_agents/random.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/user_agents/update.py
--rw-r--r--   0 runner    (1001) docker     (127)    14988 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.083664 minet-2.0.2/minet/cli/wikipedia/
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/wikipedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/wikipedia/pageviews.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.083664 minet-2.0.2/minet/cli/youtube/
--rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/youtube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/youtube/captions.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/youtube/channel_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/youtube/channel_videos.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/youtube/channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/youtube/comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/youtube/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cli/youtube/videos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-22 08:03:40.000000 minet-2.0.2/minet/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-22 08:03:40.000000 minet-2.0.2/minet/cookies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.087664 minet-2.0.2/minet/crawl/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-22 08:03:40.000000 minet-2.0.2/minet/crawl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22178 2024-04-22 08:03:40.000000 minet-2.0.2/minet/crawl/crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-22 08:03:40.000000 minet-2.0.2/minet/crawl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-04-22 08:03:40.000000 minet-2.0.2/minet/crawl/focus.py
--rw-r--r--   0 runner    (1001) docker     (127)    19409 2024-04-22 08:03:40.000000 minet-2.0.2/minet/crawl/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-22 08:03:40.000000 minet-2.0.2/minet/crawl/spiders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-22 08:03:40.000000 minet-2.0.2/minet/crawl/state.py
--rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-04-22 08:03:40.000000 minet-2.0.2/minet/crawl/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-04-22 08:03:40.000000 minet-2.0.2/minet/crawl/url_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.087664 minet-2.0.2/minet/crowdtangle/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-22 08:03:40.000000 minet-2.0.2/minet/crowdtangle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-22 08:03:40.000000 minet-2.0.2/minet/crowdtangle/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-22 08:03:40.000000 minet-2.0.2/minet/crowdtangle/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-22 08:03:40.000000 minet-2.0.2/minet/crowdtangle/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-22 08:03:40.000000 minet-2.0.2/minet/crowdtangle/leaderboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-22 08:03:40.000000 minet-2.0.2/minet/crowdtangle/lists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-22 08:03:40.000000 minet-2.0.2/minet/crowdtangle/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-22 08:03:40.000000 minet-2.0.2/minet/crowdtangle/posts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-22 08:03:40.000000 minet-2.0.2/minet/crowdtangle/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-22 08:03:40.000000 minet-2.0.2/minet/crowdtangle/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-04-22 08:03:40.000000 minet-2.0.2/minet/crowdtangle/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-04-22 08:03:40.000000 minet-2.0.2/minet/crowdtangle/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-22 08:03:40.000000 minet-2.0.2/minet/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5943 2024-04-22 08:03:40.000000 minet-2.0.2/minet/encodings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-04-22 08:03:40.000000 minet-2.0.2/minet/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    24295 2024-04-22 08:03:40.000000 minet-2.0.2/minet/executors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-22 08:03:40.000000 minet-2.0.2/minet/extraction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.091664 minet-2.0.2/minet/facebook/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-22 08:03:40.000000 minet-2.0.2/minet/facebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-22 08:03:40.000000 minet-2.0.2/minet/facebook/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-04-22 08:03:40.000000 minet-2.0.2/minet/facebook/emulated_scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-22 08:03:40.000000 minet-2.0.2/minet/facebook/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    24997 2024-04-22 08:03:40.000000 minet-2.0.2/minet/facebook/mobile_scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-22 08:03:40.000000 minet-2.0.2/minet/facebook/post_id_from_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-04-22 08:03:40.000000 minet-2.0.2/minet/facebook/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-22 08:03:40.000000 minet-2.0.2/minet/facebook/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8754 2024-04-22 08:03:40.000000 minet-2.0.2/minet/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.091664 minet-2.0.2/minet/google/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-22 08:03:40.000000 minet-2.0.2/minet/google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-22 08:03:40.000000 minet-2.0.2/minet/google/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-22 08:03:40.000000 minet-2.0.2/minet/google/sheets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-22 08:03:40.000000 minet-2.0.2/minet/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-22 08:03:40.000000 minet-2.0.2/minet/heuristics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.091664 minet-2.0.2/minet/hyphe/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-22 08:03:40.000000 minet-2.0.2/minet/hyphe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-04-22 08:03:40.000000 minet-2.0.2/minet/hyphe/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-22 08:03:40.000000 minet-2.0.2/minet/hyphe/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-22 08:03:40.000000 minet-2.0.2/minet/hyphe/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-22 08:03:40.000000 minet-2.0.2/minet/hyphe/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-22 08:03:40.000000 minet-2.0.2/minet/hyphe/spider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.091664 minet-2.0.2/minet/instagram/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-22 08:03:40.000000 minet-2.0.2/minet/instagram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16806 2024-04-22 08:03:40.000000 minet-2.0.2/minet/instagram/api_scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-22 08:03:40.000000 minet-2.0.2/minet/instagram/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-22 08:03:40.000000 minet-2.0.2/minet/instagram/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-04-22 08:03:40.000000 minet-2.0.2/minet/instagram/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-22 08:03:40.000000 minet-2.0.2/minet/instagram/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-22 08:03:40.000000 minet-2.0.2/minet/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.091664 minet-2.0.2/minet/mediacloud/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-22 08:03:40.000000 minet-2.0.2/minet/mediacloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-22 08:03:40.000000 minet-2.0.2/minet/mediacloud/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-22 08:03:40.000000 minet-2.0.2/minet/mediacloud/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-22 08:03:40.000000 minet-2.0.2/minet/mediacloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-22 08:03:40.000000 minet-2.0.2/minet/mediacloud/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-22 08:03:40.000000 minet-2.0.2/minet/mediacloud/topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-04-22 08:03:40.000000 minet-2.0.2/minet/mediacloud/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-22 08:03:40.000000 minet-2.0.2/minet/mediacloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-22 08:03:40.000000 minet-2.0.2/minet/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-04-22 08:03:40.000000 minet-2.0.2/minet/pycurl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-04-22 08:03:40.000000 minet-2.0.2/minet/rate_limiting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.095664 minet-2.0.2/minet/scrape/
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-22 08:03:40.000000 minet-2.0.2/minet/scrape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-04-22 08:03:40.000000 minet-2.0.2/minet/scrape/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.095664 minet-2.0.2/minet/scrape/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-22 08:03:40.000000 minet-2.0.2/minet/scrape/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-22 08:03:40.000000 minet-2.0.2/minet/scrape/classes/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-22 08:03:40.000000 minet-2.0.2/minet/scrape/classes/definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-22 08:03:40.000000 minet-2.0.2/minet/scrape/classes/function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.095664 minet-2.0.2/minet/scrape/classes/named/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-22 08:03:40.000000 minet-2.0.2/minet/scrape/classes/named/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-22 08:03:40.000000 minet-2.0.2/minet/scrape/classes/named/canonical.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-22 08:03:40.000000 minet-2.0.2/minet/scrape/classes/named/europresse.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-22 08:03:40.000000 minet-2.0.2/minet/scrape/classes/named/images.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-22 08:03:40.000000 minet-2.0.2/minet/scrape/classes/named/metas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-22 08:03:40.000000 minet-2.0.2/minet/scrape/classes/named/rss.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-22 08:03:40.000000 minet-2.0.2/minet/scrape/classes/named/title.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-22 08:03:40.000000 minet-2.0.2/minet/scrape/classes/named/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-22 08:03:40.000000 minet-2.0.2/minet/scrape/classes/named/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-04-22 08:03:40.000000 minet-2.0.2/minet/scrape/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-22 08:03:40.000000 minet-2.0.2/minet/scrape/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-22 08:03:40.000000 minet-2.0.2/minet/scrape/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11035 2024-04-22 08:03:40.000000 minet-2.0.2/minet/scrape/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-22 08:03:40.000000 minet-2.0.2/minet/scrape/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-22 08:03:40.000000 minet-2.0.2/minet/scrape/soup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-22 08:03:40.000000 minet-2.0.2/minet/scrape/std.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-22 08:03:40.000000 minet-2.0.2/minet/scrape/straining.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-22 08:03:40.000000 minet-2.0.2/minet/scrape/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-22 08:03:40.000000 minet-2.0.2/minet/scrape/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-22 08:03:40.000000 minet-2.0.2/minet/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-22 08:03:40.000000 minet-2.0.2/minet/sqlar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.099664 minet-2.0.2/minet/telegram/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-22 08:03:40.000000 minet-2.0.2/minet/telegram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-22 08:03:40.000000 minet-2.0.2/minet/telegram/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-22 08:03:40.000000 minet-2.0.2/minet/telegram/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12510 2024-04-22 08:03:40.000000 minet-2.0.2/minet/telegram/scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-22 08:03:40.000000 minet-2.0.2/minet/telegram/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.099664 minet-2.0.2/minet/tiktok/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-22 08:03:40.000000 minet-2.0.2/minet/tiktok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-22 08:03:40.000000 minet-2.0.2/minet/tiktok/api_scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-22 08:03:40.000000 minet-2.0.2/minet/tiktok/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-22 08:03:40.000000 minet-2.0.2/minet/tiktok/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-22 08:03:40.000000 minet-2.0.2/minet/tiktok/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.099664 minet-2.0.2/minet/twitter/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-22 08:03:40.000000 minet-2.0.2/minet/twitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-22 08:03:40.000000 minet-2.0.2/minet/twitter/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    36164 2024-04-22 08:03:40.000000 minet-2.0.2/minet/twitter/api_scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-22 08:03:40.000000 minet-2.0.2/minet/twitter/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-22 08:03:40.000000 minet-2.0.2/minet/twitter/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-22 08:03:40.000000 minet-2.0.2/minet/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.099664 minet-2.0.2/minet/user_agents/
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-22 08:03:40.000000 minet-2.0.2/minet/user_agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-22 08:03:40.000000 minet-2.0.2/minet/user_agents/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-22 08:03:40.000000 minet-2.0.2/minet/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    40611 2024-04-22 08:03:40.000000 minet-2.0.2/minet/web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.099664 minet-2.0.2/minet/wikipedia/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-22 08:03:40.000000 minet-2.0.2/minet/wikipedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-22 08:03:40.000000 minet-2.0.2/minet/wikipedia/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-22 08:03:40.000000 minet-2.0.2/minet/wikipedia/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-22 08:03:40.000000 minet-2.0.2/minet/wikipedia/wikimedia_rest_api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.099664 minet-2.0.2/minet/youtube/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-22 08:03:40.000000 minet-2.0.2/minet/youtube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13238 2024-04-22 08:03:40.000000 minet-2.0.2/minet/youtube/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-22 08:03:40.000000 minet-2.0.2/minet/youtube/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-22 08:03:40.000000 minet-2.0.2/minet/youtube/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-04-22 08:03:40.000000 minet-2.0.2/minet/youtube/scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-22 08:03:40.000000 minet-2.0.2/minet/youtube/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-22 08:03:40.000000 minet-2.0.2/minet/youtube/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-22 08:03:40.000000 minet-2.0.2/minet/youtube/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:04:56.103664 minet-2.0.2/minet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-04-22 08:04:55.000000 minet-2.0.2/minet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-04-22 08:04:56.000000 minet-2.0.2/minet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 08:04:55.000000 minet-2.0.2/minet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-22 08:04:55.000000 minet-2.0.2/minet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-22 08:04:55.000000 minet-2.0.2/minet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 08:04:55.000000 minet-2.0.2/minet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 08:04:55.000000 minet-2.0.2/minet.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 08:04:56.103664 minet-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-22 08:03:40.000000 minet-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.363597 minet-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 08:31:37.000000 minet-2.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-04-24 08:33:03.363597 minet-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-04-24 08:31:37.000000 minet-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.323597 minet-2.0.3/minet/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 08:31:37.000000 minet-2.0.3/minet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-24 08:31:37.000000 minet-2.0.3/minet/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.327597 minet-2.0.3/minet/browser/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-24 08:31:37.000000 minet-2.0.3/minet/browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-24 08:31:37.000000 minet-2.0.3/minet/browser/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-24 08:31:37.000000 minet-2.0.3/minet/browser/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-24 08:31:37.000000 minet-2.0.3/minet/browser/plawright_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11839 2024-04-24 08:31:37.000000 minet-2.0.3/minet/browser/threadsafe_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-24 08:31:37.000000 minet-2.0.3/minet/browser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.327597 minet-2.0.3/minet/buzzsumo/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-24 08:31:37.000000 minet-2.0.3/minet/buzzsumo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-24 08:31:37.000000 minet-2.0.3/minet/buzzsumo/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-24 08:31:37.000000 minet-2.0.3/minet/buzzsumo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-04-24 08:31:37.000000 minet-2.0.3/minet/buzzsumo/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.331597 minet-2.0.3/minet/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30498 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/argparse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.331597 minet-2.0.3/minet/cli/buzzsumo/
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/buzzsumo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/buzzsumo/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/buzzsumo/domain_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/buzzsumo/exact_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/buzzsumo/limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/buzzsumo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.331597 minet-2.0.3/minet/cli/cookies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/cookies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/cookies/cookies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.331597 minet-2.0.3/minet/cli/crawl/
+-rw-r--r--   0 runner    (1001) docker     (127)    14843 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/crawl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12602 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/crawl/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/crawl/focus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.331597 minet-2.0.3/minet/cli/crowdtangle/
+-rw-r--r--   0 runner    (1001) docker     (127)    11696 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/crowdtangle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/crowdtangle/leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/crowdtangle/lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/crowdtangle/posts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/crowdtangle/posts_by_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/crowdtangle/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/crowdtangle/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/crowdtangle/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.331597 minet-2.0.3/minet/cli/dump/
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/dump/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/dump/dump_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/dump/dump_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/dump/dump_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.331597 minet-2.0.3/minet/cli/extract/
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/extract/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.335597 minet-2.0.3/minet/cli/facebook/
+-rw-r--r--   0 runner    (1001) docker     (127)    10645 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/facebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/facebook/comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/facebook/experimental_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/facebook/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/facebook/post_authors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7355 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/facebook/post_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/facebook/posts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/facebook/url_likes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/facebook/user_infos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/facebook/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.335597 minet-2.0.3/minet/cli/fetch/
+-rw-r--r--   0 runner    (1001) docker     (127)    14730 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/fetch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18311 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/fetch/fetch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.335597 minet-2.0.3/minet/cli/google/
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/google/sheets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.335597 minet-2.0.3/minet/cli/hyphe/
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/hyphe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/hyphe/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/hyphe/declare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/hyphe/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/hyphe/dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/hyphe/reset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/hyphe/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/hyphe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.339597 minet-2.0.3/minet/cli/instagram/
+-rw-r--r--   0 runner    (1001) docker     (127)    11067 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/instagram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/instagram/comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/instagram/hashtag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/instagram/post_infos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/instagram/user_followers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/instagram/user_following.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/instagram/user_infos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/instagram/user_posts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/instagram/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15677 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/loading_bar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.339597 minet-2.0.3/minet/cli/mediacloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/mediacloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/mediacloud/medias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/mediacloud/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.339597 minet-2.0.3/minet/cli/mediacloud/topic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/mediacloud/topic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/mediacloud/topic/stories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/mediacloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/reporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.339597 minet-2.0.3/minet/cli/scrape/
+-rw-r--r--   0 runner    (1001) docker     (127)     8280 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/scrape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/scrape/scrape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.339597 minet-2.0.3/minet/cli/telegram/
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/telegram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/telegram/channel_infos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/telegram/channel_messages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.339597 minet-2.0.3/minet/cli/tiktok/
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/tiktok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/tiktok/search_videos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.343597 minet-2.0.3/minet/cli/twitter/
+-rw-r--r--   0 runner    (1001) docker     (127)    24913 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/twitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10869 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/twitter/attrition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/twitter/followers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/twitter/followers_you_know.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/twitter/friends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/twitter/legacy_tweets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/twitter/list_followers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/twitter/list_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/twitter/retweeters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/twitter/scrape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/twitter/tweet_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/twitter/tweet_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/twitter/tweet_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/twitter/tweets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/twitter/user_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/twitter/user_tweets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/twitter/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8182 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/twitter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.343597 minet-2.0.3/minet/cli/url_extract/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/url_extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/url_extract/url_extract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.343597 minet-2.0.3/minet/cli/url_join/
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/url_join/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/url_join/url_join.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.343597 minet-2.0.3/minet/cli/url_parse/
+-rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/url_parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/url_parse/url_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.343597 minet-2.0.3/minet/cli/user_agents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/user_agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/user_agents/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/user_agents/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/user_agents/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14988 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.343597 minet-2.0.3/minet/cli/wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/wikipedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/wikipedia/pageviews.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.343597 minet-2.0.3/minet/cli/youtube/
+-rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/youtube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/youtube/captions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/youtube/channel_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/youtube/channel_videos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/youtube/channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/youtube/comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/youtube/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cli/youtube/videos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-24 08:31:37.000000 minet-2.0.3/minet/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-24 08:31:37.000000 minet-2.0.3/minet/cookies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.347597 minet-2.0.3/minet/crawl/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-24 08:31:37.000000 minet-2.0.3/minet/crawl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22178 2024-04-24 08:31:37.000000 minet-2.0.3/minet/crawl/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-24 08:31:37.000000 minet-2.0.3/minet/crawl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-04-24 08:31:37.000000 minet-2.0.3/minet/crawl/focus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19409 2024-04-24 08:31:37.000000 minet-2.0.3/minet/crawl/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-24 08:31:37.000000 minet-2.0.3/minet/crawl/spiders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-24 08:31:37.000000 minet-2.0.3/minet/crawl/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-04-24 08:31:37.000000 minet-2.0.3/minet/crawl/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-04-24 08:31:37.000000 minet-2.0.3/minet/crawl/url_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.347597 minet-2.0.3/minet/crowdtangle/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-24 08:31:37.000000 minet-2.0.3/minet/crowdtangle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-24 08:31:37.000000 minet-2.0.3/minet/crowdtangle/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-24 08:31:37.000000 minet-2.0.3/minet/crowdtangle/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-24 08:31:37.000000 minet-2.0.3/minet/crowdtangle/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-24 08:31:37.000000 minet-2.0.3/minet/crowdtangle/leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-24 08:31:37.000000 minet-2.0.3/minet/crowdtangle/lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-24 08:31:37.000000 minet-2.0.3/minet/crowdtangle/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-24 08:31:37.000000 minet-2.0.3/minet/crowdtangle/posts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-24 08:31:37.000000 minet-2.0.3/minet/crowdtangle/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-24 08:31:37.000000 minet-2.0.3/minet/crowdtangle/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-04-24 08:31:37.000000 minet-2.0.3/minet/crowdtangle/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-04-24 08:31:37.000000 minet-2.0.3/minet/crowdtangle/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-24 08:31:37.000000 minet-2.0.3/minet/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5943 2024-04-24 08:31:37.000000 minet-2.0.3/minet/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-04-24 08:31:37.000000 minet-2.0.3/minet/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24295 2024-04-24 08:31:37.000000 minet-2.0.3/minet/executors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-24 08:31:37.000000 minet-2.0.3/minet/extraction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.351597 minet-2.0.3/minet/facebook/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-24 08:31:37.000000 minet-2.0.3/minet/facebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-24 08:31:37.000000 minet-2.0.3/minet/facebook/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-04-24 08:31:37.000000 minet-2.0.3/minet/facebook/emulated_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-24 08:31:37.000000 minet-2.0.3/minet/facebook/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24997 2024-04-24 08:31:37.000000 minet-2.0.3/minet/facebook/mobile_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-24 08:31:37.000000 minet-2.0.3/minet/facebook/post_id_from_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-04-24 08:31:37.000000 minet-2.0.3/minet/facebook/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-24 08:31:37.000000 minet-2.0.3/minet/facebook/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8754 2024-04-24 08:31:37.000000 minet-2.0.3/minet/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.351597 minet-2.0.3/minet/google/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-24 08:31:37.000000 minet-2.0.3/minet/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-24 08:31:37.000000 minet-2.0.3/minet/google/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-24 08:31:37.000000 minet-2.0.3/minet/google/sheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-24 08:31:37.000000 minet-2.0.3/minet/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-24 08:31:37.000000 minet-2.0.3/minet/heuristics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.351597 minet-2.0.3/minet/hyphe/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-24 08:31:37.000000 minet-2.0.3/minet/hyphe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-04-24 08:31:37.000000 minet-2.0.3/minet/hyphe/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-24 08:31:37.000000 minet-2.0.3/minet/hyphe/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-24 08:31:37.000000 minet-2.0.3/minet/hyphe/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-24 08:31:37.000000 minet-2.0.3/minet/hyphe/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-24 08:31:37.000000 minet-2.0.3/minet/hyphe/spider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.351597 minet-2.0.3/minet/instagram/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-24 08:31:37.000000 minet-2.0.3/minet/instagram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16806 2024-04-24 08:31:37.000000 minet-2.0.3/minet/instagram/api_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-24 08:31:37.000000 minet-2.0.3/minet/instagram/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-24 08:31:37.000000 minet-2.0.3/minet/instagram/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-04-24 08:31:37.000000 minet-2.0.3/minet/instagram/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-24 08:31:37.000000 minet-2.0.3/minet/instagram/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-24 08:31:37.000000 minet-2.0.3/minet/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.351597 minet-2.0.3/minet/mediacloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-24 08:31:37.000000 minet-2.0.3/minet/mediacloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-24 08:31:37.000000 minet-2.0.3/minet/mediacloud/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-24 08:31:37.000000 minet-2.0.3/minet/mediacloud/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-24 08:31:37.000000 minet-2.0.3/minet/mediacloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-24 08:31:37.000000 minet-2.0.3/minet/mediacloud/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-24 08:31:37.000000 minet-2.0.3/minet/mediacloud/topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-04-24 08:31:37.000000 minet-2.0.3/minet/mediacloud/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-24 08:31:37.000000 minet-2.0.3/minet/mediacloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-24 08:31:37.000000 minet-2.0.3/minet/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-04-24 08:31:37.000000 minet-2.0.3/minet/pycurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-04-24 08:31:37.000000 minet-2.0.3/minet/rate_limiting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.355597 minet-2.0.3/minet/scrape/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-24 08:31:37.000000 minet-2.0.3/minet/scrape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-04-24 08:31:37.000000 minet-2.0.3/minet/scrape/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.355597 minet-2.0.3/minet/scrape/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-24 08:31:37.000000 minet-2.0.3/minet/scrape/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-24 08:31:37.000000 minet-2.0.3/minet/scrape/classes/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-24 08:31:37.000000 minet-2.0.3/minet/scrape/classes/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-24 08:31:37.000000 minet-2.0.3/minet/scrape/classes/function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.355597 minet-2.0.3/minet/scrape/classes/named/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-24 08:31:37.000000 minet-2.0.3/minet/scrape/classes/named/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-24 08:31:37.000000 minet-2.0.3/minet/scrape/classes/named/canonical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-24 08:31:37.000000 minet-2.0.3/minet/scrape/classes/named/europresse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-24 08:31:37.000000 minet-2.0.3/minet/scrape/classes/named/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-24 08:31:37.000000 minet-2.0.3/minet/scrape/classes/named/metas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-24 08:31:37.000000 minet-2.0.3/minet/scrape/classes/named/rss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-24 08:31:37.000000 minet-2.0.3/minet/scrape/classes/named/title.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-24 08:31:37.000000 minet-2.0.3/minet/scrape/classes/named/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-24 08:31:37.000000 minet-2.0.3/minet/scrape/classes/named/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-04-24 08:31:37.000000 minet-2.0.3/minet/scrape/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-24 08:31:37.000000 minet-2.0.3/minet/scrape/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-24 08:31:37.000000 minet-2.0.3/minet/scrape/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11035 2024-04-24 08:31:37.000000 minet-2.0.3/minet/scrape/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-24 08:31:37.000000 minet-2.0.3/minet/scrape/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-24 08:31:37.000000 minet-2.0.3/minet/scrape/soup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-24 08:31:37.000000 minet-2.0.3/minet/scrape/std.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-24 08:31:37.000000 minet-2.0.3/minet/scrape/straining.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-24 08:31:37.000000 minet-2.0.3/minet/scrape/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-24 08:31:37.000000 minet-2.0.3/minet/scrape/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-24 08:31:37.000000 minet-2.0.3/minet/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-24 08:31:37.000000 minet-2.0.3/minet/sqlar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.355597 minet-2.0.3/minet/telegram/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-24 08:31:37.000000 minet-2.0.3/minet/telegram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-24 08:31:37.000000 minet-2.0.3/minet/telegram/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-24 08:31:37.000000 minet-2.0.3/minet/telegram/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12510 2024-04-24 08:31:37.000000 minet-2.0.3/minet/telegram/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-24 08:31:37.000000 minet-2.0.3/minet/telegram/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.359597 minet-2.0.3/minet/tiktok/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-24 08:31:37.000000 minet-2.0.3/minet/tiktok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-24 08:31:37.000000 minet-2.0.3/minet/tiktok/api_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-24 08:31:37.000000 minet-2.0.3/minet/tiktok/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-24 08:31:37.000000 minet-2.0.3/minet/tiktok/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-24 08:31:37.000000 minet-2.0.3/minet/tiktok/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.359597 minet-2.0.3/minet/twitter/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-24 08:31:37.000000 minet-2.0.3/minet/twitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-24 08:31:37.000000 minet-2.0.3/minet/twitter/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36164 2024-04-24 08:31:37.000000 minet-2.0.3/minet/twitter/api_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-24 08:31:37.000000 minet-2.0.3/minet/twitter/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-24 08:31:37.000000 minet-2.0.3/minet/twitter/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-24 08:31:37.000000 minet-2.0.3/minet/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.359597 minet-2.0.3/minet/user_agents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-24 08:31:37.000000 minet-2.0.3/minet/user_agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-24 08:31:37.000000 minet-2.0.3/minet/user_agents/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-24 08:31:37.000000 minet-2.0.3/minet/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40935 2024-04-24 08:31:37.000000 minet-2.0.3/minet/web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.359597 minet-2.0.3/minet/wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 08:31:37.000000 minet-2.0.3/minet/wikipedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-24 08:31:37.000000 minet-2.0.3/minet/wikipedia/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-24 08:31:37.000000 minet-2.0.3/minet/wikipedia/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-24 08:31:37.000000 minet-2.0.3/minet/wikipedia/wikimedia_rest_api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.359597 minet-2.0.3/minet/youtube/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-24 08:31:37.000000 minet-2.0.3/minet/youtube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13238 2024-04-24 08:31:37.000000 minet-2.0.3/minet/youtube/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-24 08:31:37.000000 minet-2.0.3/minet/youtube/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-24 08:31:37.000000 minet-2.0.3/minet/youtube/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-04-24 08:31:37.000000 minet-2.0.3/minet/youtube/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-24 08:31:37.000000 minet-2.0.3/minet/youtube/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-24 08:31:37.000000 minet-2.0.3/minet/youtube/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-24 08:31:37.000000 minet-2.0.3/minet/youtube/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:03.359597 minet-2.0.3/minet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-04-24 08:33:03.000000 minet-2.0.3/minet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-04-24 08:33:03.000000 minet-2.0.3/minet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:33:03.000000 minet-2.0.3/minet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-24 08:33:03.000000 minet-2.0.3/minet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-24 08:33:03.000000 minet-2.0.3/minet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 08:33:03.000000 minet-2.0.3/minet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:33:03.000000 minet-2.0.3/minet.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 08:33:03.363597 minet-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-24 08:31:37.000000 minet-2.0.3/setup.py
```

### Comparing `minet-2.0.2/LICENSE.txt` & `minet-2.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/PKG-INFO` & `minet-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minet
-Version: 2.0.2
+Version: 2.0.3
 Summary: A webmining CLI tool & library for python.
 Home-page: http://github.com/medialab/minet
 Author: Guillaume Plique, Pauline Breteau, Jules Farjas, Héloïse Théro, Jean Descamps, Amélie Pellé, Laura Miguel, César Pichon, Kelly Christensen
 License: GPL-3.0
 Keywords: webmining
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `minet-2.0.2/README.md` & `minet-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/browser/extensions.py` & `minet-2.0.3/minet/browser/extensions.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/browser/plawright_shim.py` & `minet-2.0.3/minet/browser/plawright_shim.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/browser/threadsafe_browser.py` & `minet-2.0.3/minet/browser/threadsafe_browser.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/browser/utils.py` & `minet-2.0.3/minet/browser/utils.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/buzzsumo/client.py` & `minet-2.0.3/minet/buzzsumo/client.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/buzzsumo/exceptions.py` & `minet-2.0.3/minet/buzzsumo/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/buzzsumo/types.py` & `minet-2.0.3/minet/buzzsumo/types.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/argparse.py` & `minet-2.0.3/minet/cli/argparse.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/buzzsumo/__init__.py` & `minet-2.0.3/minet/cli/buzzsumo/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/buzzsumo/domain.py` & `minet-2.0.3/minet/cli/buzzsumo/domain.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/buzzsumo/domain_summary.py` & `minet-2.0.3/minet/cli/buzzsumo/domain_summary.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/buzzsumo/exact_url.py` & `minet-2.0.3/minet/cli/buzzsumo/exact_url.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/buzzsumo/limit.py` & `minet-2.0.3/minet/cli/buzzsumo/limit.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/buzzsumo/utils.py` & `minet-2.0.3/minet/cli/buzzsumo/utils.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/commands.py` & `minet-2.0.3/minet/cli/commands.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/console.py` & `minet-2.0.3/minet/cli/console.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/cookies/__init__.py` & `minet-2.0.3/minet/cli/cookies/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/cookies/cookies.py` & `minet-2.0.3/minet/cli/cookies/cookies.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/crawl/__init__.py` & `minet-2.0.3/minet/cli/crawl/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/crawl/crawl.py` & `minet-2.0.3/minet/cli/crawl/crawl.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/crawl/focus.py` & `minet-2.0.3/minet/cli/crawl/focus.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/crowdtangle/__init__.py` & `minet-2.0.3/minet/cli/crowdtangle/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/crowdtangle/leaderboard.py` & `minet-2.0.3/minet/cli/crowdtangle/leaderboard.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/crowdtangle/lists.py` & `minet-2.0.3/minet/cli/crowdtangle/lists.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/crowdtangle/posts_by_id.py` & `minet-2.0.3/minet/cli/crowdtangle/posts_by_id.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/crowdtangle/search.py` & `minet-2.0.3/minet/cli/crowdtangle/search.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/crowdtangle/summary.py` & `minet-2.0.3/minet/cli/crowdtangle/summary.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/crowdtangle/utils.py` & `minet-2.0.3/minet/cli/crowdtangle/utils.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/dump/__init__.py` & `minet-2.0.3/minet/cli/dump/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/dump/dump_graph.py` & `minet-2.0.3/minet/cli/dump/dump_graph.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/exceptions.py` & `minet-2.0.3/minet/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/extract/__init__.py` & `minet-2.0.3/minet/cli/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/extract/extract.py` & `minet-2.0.3/minet/cli/extract/extract.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/facebook/__init__.py` & `minet-2.0.3/minet/cli/facebook/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/facebook/comments.py` & `minet-2.0.3/minet/cli/facebook/comments.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/facebook/experimental_comments.py` & `minet-2.0.3/minet/cli/facebook/experimental_comments.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/facebook/post.py` & `minet-2.0.3/minet/cli/facebook/post.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/facebook/post_authors.py` & `minet-2.0.3/minet/cli/facebook/post_authors.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/facebook/post_stats.py` & `minet-2.0.3/minet/cli/facebook/post_stats.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/facebook/posts.py` & `minet-2.0.3/minet/cli/facebook/posts.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/facebook/url_likes.py` & `minet-2.0.3/minet/cli/facebook/url_likes.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/facebook/user_infos.py` & `minet-2.0.3/minet/cli/facebook/user_infos.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/facebook/utils.py` & `minet-2.0.3/minet/cli/facebook/utils.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/fetch/__init__.py` & `minet-2.0.3/minet/cli/fetch/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/fetch/fetch.py` & `minet-2.0.3/minet/cli/fetch/fetch.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/google/__init__.py` & `minet-2.0.3/minet/cli/google/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/google/sheets.py` & `minet-2.0.3/minet/cli/google/sheets.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/hyphe/__init__.py` & `minet-2.0.3/minet/cli/hyphe/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/hyphe/crawl.py` & `minet-2.0.3/minet/cli/hyphe/crawl.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/hyphe/declare.py` & `minet-2.0.3/minet/cli/hyphe/declare.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/hyphe/destroy.py` & `minet-2.0.3/minet/cli/hyphe/destroy.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/hyphe/dump.py` & `minet-2.0.3/minet/cli/hyphe/dump.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/hyphe/reset.py` & `minet-2.0.3/minet/cli/hyphe/reset.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/hyphe/tag.py` & `minet-2.0.3/minet/cli/hyphe/tag.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/instagram/__init__.py` & `minet-2.0.3/minet/cli/instagram/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/instagram/comments.py` & `minet-2.0.3/minet/cli/instagram/comments.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/instagram/hashtag.py` & `minet-2.0.3/minet/cli/instagram/hashtag.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/instagram/post_infos.py` & `minet-2.0.3/minet/cli/instagram/post_infos.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/instagram/user_followers.py` & `minet-2.0.3/minet/cli/instagram/user_followers.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/instagram/user_following.py` & `minet-2.0.3/minet/cli/instagram/user_following.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/instagram/user_infos.py` & `minet-2.0.3/minet/cli/instagram/user_infos.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/instagram/user_posts.py` & `minet-2.0.3/minet/cli/instagram/user_posts.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/instagram/utils.py` & `minet-2.0.3/minet/cli/instagram/utils.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/loading_bar.py` & `minet-2.0.3/minet/cli/loading_bar.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/mediacloud/__init__.py` & `minet-2.0.3/minet/cli/mediacloud/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/mediacloud/medias.py` & `minet-2.0.3/minet/cli/mediacloud/medias.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/mediacloud/search.py` & `minet-2.0.3/minet/cli/mediacloud/search.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/mediacloud/topic/stories.py` & `minet-2.0.3/minet/cli/mediacloud/topic/stories.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/reporters.py` & `minet-2.0.3/minet/cli/reporters.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/run.py` & `minet-2.0.3/minet/cli/run.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/scrape/__init__.py` & `minet-2.0.3/minet/cli/scrape/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/scrape/scrape.py` & `minet-2.0.3/minet/cli/scrape/scrape.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/telegram/__init__.py` & `minet-2.0.3/minet/cli/telegram/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/telegram/channel_infos.py` & `minet-2.0.3/minet/cli/telegram/channel_infos.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/telegram/channel_messages.py` & `minet-2.0.3/minet/cli/telegram/channel_messages.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/tiktok/__init__.py` & `minet-2.0.3/minet/cli/tiktok/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/tiktok/search_videos.py` & `minet-2.0.3/minet/cli/tiktok/search_videos.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/twitter/__init__.py` & `minet-2.0.3/minet/cli/twitter/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/twitter/attrition.py` & `minet-2.0.3/minet/cli/twitter/attrition.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/twitter/followers_you_know.py` & `minet-2.0.3/minet/cli/twitter/followers_you_know.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/twitter/legacy_tweets.py` & `minet-2.0.3/minet/cli/twitter/legacy_tweets.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/twitter/list_followers.py` & `minet-2.0.3/minet/cli/twitter/list_followers.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/twitter/list_members.py` & `minet-2.0.3/minet/cli/twitter/list_members.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/twitter/retweeters.py` & `minet-2.0.3/minet/cli/twitter/retweeters.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/twitter/scrape.py` & `minet-2.0.3/minet/cli/twitter/scrape.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/twitter/tweet_count.py` & `minet-2.0.3/minet/cli/twitter/tweet_count.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/twitter/tweet_date.py` & `minet-2.0.3/minet/cli/twitter/tweet_date.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/twitter/tweet_search.py` & `minet-2.0.3/minet/cli/twitter/tweet_search.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/twitter/tweets.py` & `minet-2.0.3/minet/cli/twitter/tweets.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/twitter/user_search.py` & `minet-2.0.3/minet/cli/twitter/user_search.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/twitter/user_tweets.py` & `minet-2.0.3/minet/cli/twitter/user_tweets.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/twitter/users.py` & `minet-2.0.3/minet/cli/twitter/users.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/twitter/utils.py` & `minet-2.0.3/minet/cli/twitter/utils.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/url_extract/__init__.py` & `minet-2.0.3/minet/cli/url_extract/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/url_extract/url_extract.py` & `minet-2.0.3/minet/cli/url_extract/url_extract.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/url_join/__init__.py` & `minet-2.0.3/minet/cli/url_join/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/url_join/url_join.py` & `minet-2.0.3/minet/cli/url_join/url_join.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/url_parse/__init__.py` & `minet-2.0.3/minet/cli/url_parse/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/url_parse/url_parse.py` & `minet-2.0.3/minet/cli/url_parse/url_parse.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/user_agents/__init__.py` & `minet-2.0.3/minet/cli/user_agents/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/utils.py` & `minet-2.0.3/minet/cli/utils.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/wikipedia/__init__.py` & `minet-2.0.3/minet/cli/wikipedia/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/wikipedia/pageviews.py` & `minet-2.0.3/minet/cli/wikipedia/pageviews.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/youtube/__init__.py` & `minet-2.0.3/minet/cli/youtube/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/youtube/captions.py` & `minet-2.0.3/minet/cli/youtube/captions.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/youtube/channel_links.py` & `minet-2.0.3/minet/cli/youtube/channel_links.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/youtube/channel_videos.py` & `minet-2.0.3/minet/cli/youtube/channel_videos.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/youtube/channels.py` & `minet-2.0.3/minet/cli/youtube/channels.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/youtube/comments.py` & `minet-2.0.3/minet/cli/youtube/comments.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/youtube/search.py` & `minet-2.0.3/minet/cli/youtube/search.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cli/youtube/videos.py` & `minet-2.0.3/minet/cli/youtube/videos.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/constants.py` & `minet-2.0.3/minet/constants.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/cookies.py` & `minet-2.0.3/minet/cookies.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/crawl/crawler.py` & `minet-2.0.3/minet/crawl/crawler.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/crawl/focus.py` & `minet-2.0.3/minet/crawl/focus.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/crawl/queue.py` & `minet-2.0.3/minet/crawl/queue.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/crawl/spiders.py` & `minet-2.0.3/minet/crawl/spiders.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/crawl/state.py` & `minet-2.0.3/minet/crawl/state.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/crawl/types.py` & `minet-2.0.3/minet/crawl/types.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/crawl/url_cache.py` & `minet-2.0.3/minet/crawl/url_cache.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/crowdtangle/client.py` & `minet-2.0.3/minet/crowdtangle/client.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/crowdtangle/constants.py` & `minet-2.0.3/minet/crowdtangle/constants.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/crowdtangle/exceptions.py` & `minet-2.0.3/minet/crowdtangle/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/crowdtangle/leaderboard.py` & `minet-2.0.3/minet/crowdtangle/leaderboard.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/crowdtangle/lists.py` & `minet-2.0.3/minet/crowdtangle/lists.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/crowdtangle/post.py` & `minet-2.0.3/minet/crowdtangle/post.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/crowdtangle/posts.py` & `minet-2.0.3/minet/crowdtangle/posts.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/crowdtangle/search.py` & `minet-2.0.3/minet/crowdtangle/search.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/crowdtangle/summary.py` & `minet-2.0.3/minet/crowdtangle/summary.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/crowdtangle/types.py` & `minet-2.0.3/minet/crowdtangle/types.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/crowdtangle/utils.py` & `minet-2.0.3/minet/crowdtangle/utils.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/dates.py` & `minet-2.0.3/minet/dates.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/encodings.py` & `minet-2.0.3/minet/encodings.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/exceptions.py` & `minet-2.0.3/minet/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,31 +241,35 @@
 
 
 # Browser emulation
 class BrowserError(MinetError):
     pass
 
 
+class BrowserProtocolError(BrowserError):
+    pass
+
+
 class BrowserYetUnimplementedError(BrowserError):
     pass
 
 
 class BrowserNameNotResolvedError(BrowserError):
     pass
 
 
-class BrowserConnectionAbortedError(BrowserError):
+class BrowserConnectionAbortedError(BrowserProtocolError):
     pass
 
 
-class BrowserConnectionRefusedError(BrowserError):
+class BrowserConnectionRefusedError(BrowserProtocolError):
     pass
 
 
-class BrowserConnectionClosedError(BrowserError):
+class BrowserConnectionClosedError(BrowserProtocolError):
     pass
 
 
 class BrowserConnectionTimeoutError(BrowserError):
     pass
 
 
@@ -273,15 +277,15 @@
     pass
 
 
 class BrowserSSLError(BrowserError):
     pass
 
 
-class BrowserHTTPResponseCodeFailureError(BrowserError):
+class BrowserHTTPResponseCodeFailureError(BrowserProtocolError):
     pass
 
 
 class BrowserContextAlreadyClosedError(BrowserError):
     pass
```

### Comparing `minet-2.0.2/minet/executors.py` & `minet-2.0.3/minet/executors.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/extraction.py` & `minet-2.0.3/minet/extraction.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/facebook/constants.py` & `minet-2.0.3/minet/facebook/constants.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/facebook/emulated_scraper.py` & `minet-2.0.3/minet/facebook/emulated_scraper.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/facebook/exceptions.py` & `minet-2.0.3/minet/facebook/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/facebook/mobile_scraper.py` & `minet-2.0.3/minet/facebook/mobile_scraper.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/facebook/post_id_from_url.py` & `minet-2.0.3/minet/facebook/post_id_from_url.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/facebook/types.py` & `minet-2.0.3/minet/facebook/types.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/facebook/utils.py` & `minet-2.0.3/minet/facebook/utils.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/fs.py` & `minet-2.0.3/minet/fs.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/google/exceptions.py` & `minet-2.0.3/minet/google/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/google/sheets.py` & `minet-2.0.3/minet/google/sheets.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/headers.py` & `minet-2.0.3/minet/headers.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/hyphe/client.py` & `minet-2.0.3/minet/hyphe/client.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/hyphe/constants.py` & `minet-2.0.3/minet/hyphe/constants.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/hyphe/exceptions.py` & `minet-2.0.3/minet/hyphe/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/hyphe/formatters.py` & `minet-2.0.3/minet/hyphe/formatters.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/hyphe/spider.py` & `minet-2.0.3/minet/hyphe/spider.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/instagram/api_scraper.py` & `minet-2.0.3/minet/instagram/api_scraper.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/instagram/constants.py` & `minet-2.0.3/minet/instagram/constants.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/instagram/exceptions.py` & `minet-2.0.3/minet/instagram/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/instagram/types.py` & `minet-2.0.3/minet/instagram/types.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/instagram/utils.py` & `minet-2.0.3/minet/instagram/utils.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/mediacloud/client.py` & `minet-2.0.3/minet/mediacloud/client.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/mediacloud/exceptions.py` & `minet-2.0.3/minet/mediacloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/mediacloud/search.py` & `minet-2.0.3/minet/mediacloud/search.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/mediacloud/topic.py` & `minet-2.0.3/minet/mediacloud/topic.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/mediacloud/types.py` & `minet-2.0.3/minet/mediacloud/types.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/mediacloud/utils.py` & `minet-2.0.3/minet/mediacloud/utils.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/multiprocessing.py` & `minet-2.0.3/minet/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/pycurl.py` & `minet-2.0.3/minet/pycurl.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/rate_limiting.py` & `minet-2.0.3/minet/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/scrape/__init__.py` & `minet-2.0.3/minet/scrape/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/scrape/analysis.py` & `minet-2.0.3/minet/scrape/analysis.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/scrape/classes/base.py` & `minet-2.0.3/minet/scrape/classes/base.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/scrape/classes/definition.py` & `minet-2.0.3/minet/scrape/classes/definition.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/scrape/classes/function.py` & `minet-2.0.3/minet/scrape/classes/function.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/scrape/classes/named/__init__.py` & `minet-2.0.3/minet/scrape/classes/named/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/scrape/classes/named/canonical.py` & `minet-2.0.3/minet/scrape/classes/named/canonical.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/scrape/classes/named/europresse.py` & `minet-2.0.3/minet/scrape/classes/named/europresse.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/scrape/classes/named/images.py` & `minet-2.0.3/minet/scrape/classes/named/images.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/scrape/classes/named/metas.py` & `minet-2.0.3/minet/scrape/classes/named/metas.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/scrape/classes/named/rss.py` & `minet-2.0.3/minet/scrape/classes/named/rss.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/scrape/classes/named/types.py` & `minet-2.0.3/minet/scrape/classes/named/types.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/scrape/classes/named/urls.py` & `minet-2.0.3/minet/scrape/classes/named/urls.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/scrape/compiler.py` & `minet-2.0.3/minet/scrape/compiler.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/scrape/constants.py` & `minet-2.0.3/minet/scrape/constants.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/scrape/exceptions.py` & `minet-2.0.3/minet/scrape/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/scrape/interpreter.py` & `minet-2.0.3/minet/scrape/interpreter.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/scrape/regex.py` & `minet-2.0.3/minet/scrape/regex.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/scrape/soup.py` & `minet-2.0.3/minet/scrape/soup.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/scrape/std.py` & `minet-2.0.3/minet/scrape/std.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/scrape/straining.py` & `minet-2.0.3/minet/scrape/straining.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/scrape/utils.py` & `minet-2.0.3/minet/scrape/utils.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/serialization.py` & `minet-2.0.3/minet/serialization.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/sqlar.py` & `minet-2.0.3/minet/sqlar.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/telegram/scraper.py` & `minet-2.0.3/minet/telegram/scraper.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/telegram/types.py` & `minet-2.0.3/minet/telegram/types.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/tiktok/api_scraper.py` & `minet-2.0.3/minet/tiktok/api_scraper.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/tiktok/exceptions.py` & `minet-2.0.3/minet/tiktok/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/tiktok/types.py` & `minet-2.0.3/minet/tiktok/types.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/twitter/api_client.py` & `minet-2.0.3/minet/twitter/api_client.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/twitter/api_scraper.py` & `minet-2.0.3/minet/twitter/api_scraper.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/twitter/constants.py` & `minet-2.0.3/minet/twitter/constants.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/twitter/exceptions.py` & `minet-2.0.3/minet/twitter/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/types.py` & `minet-2.0.3/minet/types.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/user_agents/__init__.py` & `minet-2.0.3/minet/user_agents/__init__.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/user_agents/data.py` & `minet-2.0.3/minet/user_agents/data.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/utils.py` & `minet-2.0.3/minet/utils.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/web.py` & `minet-2.0.3/minet/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,18 @@
     SelfRedirectError,
     CancelledRequestError,
     FinalTimeoutError,
     PycurlNotInstalledError,
     PycurlError,
     PycurlProtocolError,
     PycurlTimeoutError,
+    BrowserError,
+    BrowserProtocolError,
+    BrowserConnectionTimeoutError,
+    BrowserTimeoutError,
 )
 from minet.constants import (
     DEFAULT_SPOOFED_TLS_CIPHERS,
     DEFAULT_URLLIB3_TIMEOUT,
     DEFAULT_SPOOFED_UA,
     REDIRECT_STATUSES,
 )
@@ -110,14 +114,15 @@
     urllib.error.URLError,
     urllib3_exceptions.HTTPError,
     RedirectError,
     InvalidURLError,
     InvalidStatusError,
     FinalTimeoutError,
     PycurlError,
+    BrowserError,
 )
 
 assert CONTENT_PREBUFFER_UP_TO < LARGE_CONTENT_PREBUFFER_UP_TO
 
 
 def looks_like_html(html_chunk: bytes) -> bool:
     return HTML_RE.match(html_chunk) is not None
@@ -1240,20 +1245,28 @@
         urllib.error.URLError,
         # Low-level socket connection errors
         ConnectionAbortedError,
         ConnectionRefusedError,
         ConnectionResetError,
         # pycurl errors
         PycurlProtocolError,
+        # browser errors
+        BrowserProtocolError,
     ]
 
     # We also usually include most timeout errors
     if retry_on_timeout:
         retryable_exception_types.extend(
-            [FinalTimeoutError, urllib3_exceptions.TimeoutError, PycurlTimeoutError]
+            [
+                FinalTimeoutError,
+                urllib3_exceptions.TimeoutError,
+                PycurlTimeoutError,
+                BrowserTimeoutError,
+                BrowserConnectionTimeoutError,
+            ]
         )
 
     if retry_on_statuses is not None:
         retryable_exception_types.append(InvalidStatusError)
 
     if additional_exceptions:
         for exc in additional_exceptions:
```

### Comparing `minet-2.0.2/minet/wikipedia/wikimedia_rest_api_client.py` & `minet-2.0.3/minet/wikipedia/wikimedia_rest_api_client.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/youtube/client.py` & `minet-2.0.3/minet/youtube/client.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/youtube/constants.py` & `minet-2.0.3/minet/youtube/constants.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/youtube/exceptions.py` & `minet-2.0.3/minet/youtube/exceptions.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/youtube/scraper.py` & `minet-2.0.3/minet/youtube/scraper.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/youtube/types.py` & `minet-2.0.3/minet/youtube/types.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/youtube/urls.py` & `minet-2.0.3/minet/youtube/urls.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet/youtube/utils.py` & `minet-2.0.3/minet/youtube/utils.py`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/minet.egg-info/PKG-INFO` & `minet-2.0.3/minet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minet
-Version: 2.0.2
+Version: 2.0.3
 Summary: A webmining CLI tool & library for python.
 Home-page: http://github.com/medialab/minet
 Author: Guillaume Plique, Pauline Breteau, Jules Farjas, Héloïse Théro, Jean Descamps, Amélie Pellé, Laura Miguel, César Pichon, Kelly Christensen
 License: GPL-3.0
 Keywords: webmining
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `minet-2.0.2/minet.egg-info/SOURCES.txt` & `minet-2.0.3/minet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `minet-2.0.2/setup.py` & `minet-2.0.3/setup.py`

 * *Files identical despite different names*

