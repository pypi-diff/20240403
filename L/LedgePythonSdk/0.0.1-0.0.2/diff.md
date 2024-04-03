# Comparing `tmp/LedgePythonSdk-0.0.1.tar.gz` & `tmp/LedgePythonSdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LedgePythonSdk-0.0.1.tar", last modified: Tue Apr  2 17:30:35 2024, max compression
+gzip compressed data, was "LedgePythonSdk-0.0.2.tar", last modified: Wed Apr  3 19:25:00 2024, max compression
```

## Comparing `LedgePythonSdk-0.0.1.tar` & `LedgePythonSdk-0.0.2.tar`

### file list

```diff
@@ -1,241 +1,241 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:30:35.848814 LedgePythonSdk-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:30:35.848814 LedgePythonSdk-0.0.1/LedgePythonSdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-02 17:30:35.000000 LedgePythonSdk-0.0.1/LedgePythonSdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-04-02 17:30:35.000000 LedgePythonSdk-0.0.1/LedgePythonSdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 17:30:35.000000 LedgePythonSdk-0.0.1/LedgePythonSdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-02 17:30:35.000000 LedgePythonSdk-0.0.1/LedgePythonSdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 17:30:35.000000 LedgePythonSdk-0.0.1/LedgePythonSdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-02 17:30:35.848814 LedgePythonSdk-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16068 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:30:35.800815 LedgePythonSdk-0.0.1/ledge_python_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:30:35.804815 LedgePythonSdk-0.0.1/ledge_python_sdk/api/
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43352 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/api/case_reward_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    20580 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/api/draw_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    84589 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/api/external_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    79841 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/api/games_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10631 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/api/guest_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   101373 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/api/inventory_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    31590 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/api/leaderboard_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13008 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/api/listings_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    31860 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/api/notification_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    31387 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/api/product_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    65813 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/api/quests_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    21577 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/api/screens_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    63947 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/api/social_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12893 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/api/transaction_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   213450 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    25806 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15347 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:30:35.824814 LedgePythonSdk-0.0.1/ledge_python_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/activity_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/activity_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/banner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/case_reward.py
--rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/case_reward_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/connected_social.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/connection_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/create_goal_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/create_notification_token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/create_quest_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/create_quest_schedule200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/create_quest_schedule_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/create_user_installed_games_request_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/draw_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/draw_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/draw_product_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/draw_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/draw_schedule_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/external_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/external_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/game.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/game_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/game_genre.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/game_genre_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/game_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/game_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/game_tag_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/game_with_title_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/gender.py
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/genre.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/genre_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/get_profile200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/goal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/goal_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/goal_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/goal_product_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/leaderboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/listing_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/merge_account_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/notification_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/notification_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/notification_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/paginated_case_reward_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/paginated_case_reward_detailed_pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/paginated_game_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/paginated_listing_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/paginated_notification_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/paginated_quest_schedule_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/paginated_rank_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/paginated_screen_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/paginated_transaction_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/period_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/player_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/processed_draw_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/product.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/product_swap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/product_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/quest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/quest_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/quest_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/quest_schedule_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/quest_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/rank.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/rank_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/register_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/screen.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/screen_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/social_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/status_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/tag_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/track_activity200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/transaction_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/transaction_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/update_notifications_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/update_profile_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/user_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/user_draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/user_draw_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/user_inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/user_inventory_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/user_quest_draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/user_quest_draw_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/models/user_spin_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9237 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/ledge_python_sdk/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 17:30:35.848814 LedgePythonSdk-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:30:35.848814 LedgePythonSdk-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_activity_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_activity_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_banner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_case_reward.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_case_reward_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_case_reward_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_connected_social.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_connection_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_create_goal_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_create_notification_token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_create_quest_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_create_quest_schedule200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_create_quest_schedule_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_create_user_installed_games_request_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_draw.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_draw_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_draw_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_draw_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_draw_product_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_draw_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_draw_schedule_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_external_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_external_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_external_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_game.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_game_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_game_genre.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_game_genre_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_game_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_game_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_game_tag_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_game_with_title_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_games_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_gender.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_genre.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_genre_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_get_profile200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_goal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_goal_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_goal_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_goal_product_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_guest_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_inventory_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_leaderboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_leaderboard_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_listing_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_listings_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_merge_account_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_notification_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_notification_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_notification_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_notification_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_paginated_case_reward_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_paginated_case_reward_detailed_pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_paginated_game_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_paginated_listing_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_paginated_notification_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_paginated_quest_schedule_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_paginated_rank_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_paginated_screen_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_paginated_transaction_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_period_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_player_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_processed_draw_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_product.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_product_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_product_swap.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_product_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_quest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_quest_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_quest_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_quest_schedule_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_quest_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_quests_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_rank.py
--rw-r--r--   0 runner    (1001) docker     (127)     5823 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_rank_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_register_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_screen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_screen_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_screens_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_social_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_social_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_status_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_tag_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_track_activity200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_transaction_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_transaction_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_transaction_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_update_notifications_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_update_profile_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_user_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_user_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_user_draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_user_draw_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_user_inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_user_inventory_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_user_quest_draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_user_quest_draw_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-02 17:30:18.000000 LedgePythonSdk-0.0.1/test/test_user_spin_detailed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:25:00.757021 LedgePythonSdk-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:25:00.757021 LedgePythonSdk-0.0.2/LedgePythonSdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-03 19:25:00.000000 LedgePythonSdk-0.0.2/LedgePythonSdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-04-03 19:25:00.000000 LedgePythonSdk-0.0.2/LedgePythonSdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:25:00.000000 LedgePythonSdk-0.0.2/LedgePythonSdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 19:25:00.000000 LedgePythonSdk-0.0.2/LedgePythonSdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 19:25:00.000000 LedgePythonSdk-0.0.2/LedgePythonSdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-03 19:25:00.757021 LedgePythonSdk-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:25:00.689020 LedgePythonSdk-0.0.2/ledge_python_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:25:00.693020 LedgePythonSdk-0.0.2/ledge_python_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43352 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/api/case_reward_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20580 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/api/draw_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84598 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/api/external_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79841 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/api/games_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10631 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/api/guest_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101373 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/api/inventory_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31590 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/api/leaderboard_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13008 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/api/listings_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31860 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/api/notification_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31387 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/api/product_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65813 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/api/quests_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21577 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/api/screens_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63947 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/api/social_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12893 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/api/transaction_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   213450 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25815 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15356 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:25:00.713021 LedgePythonSdk-0.0.2/ledge_python_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/activity_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/activity_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/banner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/case_reward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/case_reward_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/connected_social.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/connection_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/create_goal_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/create_notification_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/create_quest_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/create_quest_schedule200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/create_quest_schedule_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/create_user_installed_games_request_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/draw_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/draw_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/draw_product_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/draw_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/draw_schedule_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/external_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/external_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/game.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/game_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/game_genre.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/game_genre_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/game_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/game_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/game_tag_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/game_with_title_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/gender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/genre.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/genre_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/get_profile200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/goal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/goal_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/goal_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/goal_product_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/listing_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/merge_account_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/notification_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/notification_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/notification_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/paginated_case_reward_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/paginated_case_reward_detailed_pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/paginated_game_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/paginated_listing_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/paginated_notification_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/paginated_quest_schedule_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/paginated_rank_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/paginated_screen_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/paginated_transaction_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/period_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/player_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/processed_draw_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/product_swap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/product_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/quest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/quest_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/quest_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/quest_schedule_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/quest_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/rank_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/register_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/screen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/screen_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/social_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/status_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/tag_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/track_activity200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/transaction_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/transaction_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/update_notifications_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/update_profile_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/user_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/user_draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/user_draw_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/user_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/user_inventory_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/user_quest_draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/user_quest_draw_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/models/user_spin_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/ledge_python_sdk/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-03 19:25:00.757021 LedgePythonSdk-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:25:00.757021 LedgePythonSdk-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_activity_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_activity_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_banner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_case_reward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_case_reward_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_case_reward_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_connected_social.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_connection_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_create_goal_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_create_notification_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_create_quest_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_create_quest_schedule200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_create_quest_schedule_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_create_user_installed_games_request_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_draw_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_draw_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_draw_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_draw_product_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_draw_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_draw_schedule_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_external_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_external_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_external_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_game.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_game_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_game_genre.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_game_genre_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_game_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_game_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_game_tag_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_game_with_title_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_games_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_gender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_genre.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_genre_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_get_profile200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_goal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_goal_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_goal_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_goal_product_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_guest_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_inventory_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_leaderboard_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_listing_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_listings_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_merge_account_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_notification_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_notification_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_notification_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_notification_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_paginated_case_reward_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_paginated_case_reward_detailed_pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_paginated_game_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_paginated_listing_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_paginated_notification_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_paginated_quest_schedule_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_paginated_rank_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_paginated_screen_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_paginated_transaction_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_period_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_player_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_processed_draw_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_product_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_product_swap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_product_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_quest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_quest_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_quest_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_quest_schedule_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_quest_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_quests_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5823 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_rank_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_register_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_screen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_screen_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_screens_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_social_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_social_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_status_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_tag_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_track_activity200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_transaction_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_transaction_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_transaction_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_update_notifications_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_update_profile_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_user_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_user_draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_user_draw_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_user_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_user_inventory_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_user_quest_draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_user_quest_draw_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-03 19:24:56.000000 LedgePythonSdk-0.0.2/test/test_user_spin_detailed.py
```

### Comparing `LedgePythonSdk-0.0.1/LedgePythonSdk.egg-info/PKG-INFO` & `LedgePythonSdk-0.0.2/LedgePythonSdk.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: LedgePythonSdk
-Version: 0.0.1
-Summary: @ledge/api
+Version: 0.0.2
+Summary: @ledge/external-api
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 License: MIT
-Keywords: OpenAPI,OpenAPI-Generator,@ledge/api
+Keywords: OpenAPI,OpenAPI-Generator,@ledge/external-api
 Description-Content-Type: text/markdown
 Requires-Dist: urllib3<2.1.0,>=1.25.3
 Requires-Dist: python-dateutil
 Requires-Dist: pydantic>=2
 Requires-Dist: typing-extensions>=4.7.1
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
```

### Comparing `LedgePythonSdk-0.0.1/LedgePythonSdk.egg-info/SOURCES.txt` & `LedgePythonSdk-0.0.2/LedgePythonSdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/PKG-INFO` & `LedgePythonSdk-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: LedgePythonSdk
-Version: 0.0.1
-Summary: @ledge/api
+Version: 0.0.2
+Summary: @ledge/external-api
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 License: MIT
-Keywords: OpenAPI,OpenAPI-Generator,@ledge/api
+Keywords: OpenAPI,OpenAPI-Generator,@ledge/external-api
 Description-Content-Type: text/markdown
 Requires-Dist: urllib3<2.1.0,>=1.25.3
 Requires-Dist: python-dateutil
 Requires-Dist: pydantic>=2
 Requires-Dist: typing-extensions>=4.7.1
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
```

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/api/case_reward_api.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/api/case_reward_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/api/draw_api.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/api/draw_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/api/external_api.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/api/external_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    @ledge/api
+    @ledge/external-api
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.0.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
```

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/api/games_api.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/api/games_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/api/guest_api.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/api/guest_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/api/inventory_api.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/api/inventory_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/api/leaderboard_api.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/api/leaderboard_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/api/listings_api.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/api/listings_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/api/notification_api.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/api/notification_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/api/product_api.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/api/product_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/api/quests_api.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/api/quests_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/api/screens_api.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/api/screens_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/api/social_api.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/api/social_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/api/transaction_api.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/api/transaction_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/api/user_api.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/api/user_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/api_client.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    @ledge/api
+    @ledge/external-api
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.0.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -83,15 +83,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.0.1/python'
+        self.user_agent = 'OpenAPI-Generator/0.0.2/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/api_response.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/api_response.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/configuration.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    @ledge/api
+    @ledge/external-api
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.0.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -395,15 +395,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 0.0.1".\
+               "SDK Package Version: 0.0.2".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/exceptions.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    @ledge/api
+    @ledge/external-api
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.0.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
```

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/activity.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/activity.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/activity_input.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/activity_input.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/activity_type.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/activity_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    @ledge/api
+    @ledge/external-api
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.0.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
```

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/banner.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/banner.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/case_reward.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/case_reward.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/case_reward_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/case_reward_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/connected_social.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/connected_social.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/connection_type.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/connection_type.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/create_goal_request.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/create_goal_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    @ledge/api
+    @ledge/external-api
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.0.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
```

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/create_notification_token_request.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/create_notification_token_request.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/create_quest_request.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/create_quest_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    @ledge/api
+    @ledge/external-api
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.0.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
```

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/create_quest_schedule200_response.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/create_quest_schedule200_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    @ledge/api
+    @ledge/external-api
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.0.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
```

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/create_quest_schedule_request.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/create_quest_schedule_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    @ledge/api
+    @ledge/external-api
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.0.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
```

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/create_user_installed_games_request_inner.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/create_user_installed_games_request_inner.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/draw.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/draw.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/draw_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/draw_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/draw_product.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/draw_product.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/draw_product_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/draw_product_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/draw_schedule.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/draw_schedule.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/draw_schedule_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/draw_schedule_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/error_response.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/error_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    @ledge/api
+    @ledge/external-api
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.0.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
```

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/external_activity.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/external_activity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    @ledge/api
+    @ledge/external-api
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.0.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
```

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/external_user.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/external_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    @ledge/api
+    @ledge/external-api
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.0.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
```

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/game.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/game.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/game_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/game_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/game_genre.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/game_genre.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/game_genre_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/game_genre_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/game_images.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/game_images.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/game_tag.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/game_tag.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/game_tag_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/game_tag_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/game_with_title_icon.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/game_with_title_icon.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/gender.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/gender.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    @ledge/api
+    @ledge/external-api
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.0.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
```

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/genre.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/genre.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/genre_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/genre_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/get_profile200_response.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/get_profile200_response.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/goal.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/goal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    @ledge/api
+    @ledge/external-api
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.0.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
```

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/goal_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/goal_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/goal_product.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/goal_product.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/goal_product_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/goal_product_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/leaderboard.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/leaderboard.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/listing.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/listing.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/listing_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/listing_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/merge_account_request.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/merge_account_request.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/notification.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/notification.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/notification_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/notification_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/notification_token.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/notification_token.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/notification_type.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/notification_type.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/paginated_case_reward_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/paginated_case_reward_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/paginated_case_reward_detailed_pagination.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/paginated_case_reward_detailed_pagination.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/paginated_game_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/paginated_game_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/paginated_listing_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/paginated_listing_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/paginated_notification_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/paginated_notification_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/paginated_quest_schedule_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/paginated_quest_schedule_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/paginated_rank_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/paginated_rank_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/paginated_screen_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/paginated_screen_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/paginated_transaction_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/paginated_transaction_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/period_type.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/period_type.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/player_stats.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/player_stats.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/processed_draw_schedule.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/processed_draw_schedule.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/product.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/product.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/product_swap.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/product_swap.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/product_type.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/product_type.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/progress.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/progress.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/quest.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/quest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    @ledge/api
+    @ledge/external-api
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.0.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
```

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/quest_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/quest_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/quest_schedule.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/quest_schedule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    @ledge/api
+    @ledge/external-api
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.0.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
```

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/quest_schedule_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/quest_schedule_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/quest_type.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/transaction_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,24 +14,25 @@
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class QuestType(str, Enum):
+class TransactionType(str, Enum):
     """
-    QuestType
+    TransactionType
     """
 
     """
     allowed enum values
     """
-    INDIVIDUAL = 'INDIVIDUAL'
-    COMMUNITY = 'COMMUNITY'
+    REWARD = 'REWARD'
+    MARKETPLACE = 'MARKETPLACE'
+    DRAW = 'DRAW'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of QuestType from a JSON string"""
+        """Create an instance of TransactionType from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/rank.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/rank.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/rank_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/rank_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/register_request.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/register_request.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/screen.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/screen.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/screen_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/screen_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/social_profile.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/social_profile.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/status_type.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/status_type.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/tag.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/tag.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/tag_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/tag_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/track_activity200_response.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/track_activity200_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    @ledge/api
+    @ledge/external-api
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.0.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
```

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/transaction.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/transaction.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/transaction_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/transaction_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/transaction_type.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/quest_type.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    @ledge/api
+    @ledge/external-api
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.0.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -14,25 +14,24 @@
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class TransactionType(str, Enum):
+class QuestType(str, Enum):
     """
-    TransactionType
+    QuestType
     """
 
     """
     allowed enum values
     """
-    REWARD = 'REWARD'
-    MARKETPLACE = 'MARKETPLACE'
-    DRAW = 'DRAW'
+    INDIVIDUAL = 'INDIVIDUAL'
+    COMMUNITY = 'COMMUNITY'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of TransactionType from a JSON string"""
+        """Create an instance of QuestType from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/update_notifications_request.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/update_notifications_request.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/update_profile_request.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/update_profile_request.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/update_request.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/update_request.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/user.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    @ledge/api
+    @ledge/external-api
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.0.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
```

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/user_connection.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/user_connection.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/user_draw.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/user_draw.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/user_draw_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/user_draw_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/user_inventory.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/user_inventory.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/user_inventory_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/user_inventory_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/user_quest_draw.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/user_quest_draw.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/user_quest_draw_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/user_quest_draw_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/models/user_spin_detailed.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/models/user_spin_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/ledge_python_sdk/rest.py` & `LedgePythonSdk-0.0.2/ledge_python_sdk/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    @ledge/api
+    @ledge/external-api
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.0.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
```

### Comparing `LedgePythonSdk-0.0.1/pyproject.toml` & `LedgePythonSdk-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "ledge_python_sdk"
-version = "0.0.1"
-description = "@ledge/api"
+version = "0.0.2"
+description = "@ledge/external-api"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
-keywords = ["OpenAPI", "OpenAPI-Generator", "@ledge/api"]
+keywords = ["OpenAPI", "OpenAPI-Generator", "@ledge/external-api"]
 include = ["ledge_python_sdk/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 urllib3 = ">= 1.25.3"
 python-dateutil = ">=2.8.2"
```

### Comparing `LedgePythonSdk-0.0.1/setup.py` & `LedgePythonSdk-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    @ledge/api
+    @ledge/external-api
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
     The version of the OpenAPI document: 1.0.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
@@ -17,31 +17,31 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "LedgePythonSdk"
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
 
 setup(
     name=NAME,
     version=VERSION,
-    description="@ledge/api",
+    description="@ledge/external-api",
     author="OpenAPI Generator community",
     author_email="team@openapitools.org",
     url="",
-    keywords=["OpenAPI", "OpenAPI-Generator", "@ledge/api"],
+    keywords=["OpenAPI", "OpenAPI-Generator", "@ledge/external-api"],
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
     license="MIT",
     long_description_content_type='text/markdown',
     long_description="""\
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
```

### Comparing `LedgePythonSdk-0.0.1/test/test_activity.py` & `LedgePythonSdk-0.0.2/test/test_activity.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_activity_input.py` & `LedgePythonSdk-0.0.2/test/test_activity_input.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_activity_type.py` & `LedgePythonSdk-0.0.2/test/test_activity_type.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_banner.py` & `LedgePythonSdk-0.0.2/test/test_banner.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_case_reward.py` & `LedgePythonSdk-0.0.2/test/test_case_reward.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_case_reward_api.py` & `LedgePythonSdk-0.0.2/test/test_case_reward_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_case_reward_detailed.py` & `LedgePythonSdk-0.0.2/test/test_case_reward_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_connected_social.py` & `LedgePythonSdk-0.0.2/test/test_connected_social.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_connection_type.py` & `LedgePythonSdk-0.0.2/test/test_connection_type.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_create_goal_request.py` & `LedgePythonSdk-0.0.2/test/test_create_goal_request.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_create_notification_token_request.py` & `LedgePythonSdk-0.0.2/test/test_create_notification_token_request.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_create_quest_request.py` & `LedgePythonSdk-0.0.2/test/test_create_quest_request.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_create_quest_schedule200_response.py` & `LedgePythonSdk-0.0.2/test/test_create_quest_schedule200_response.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_create_quest_schedule_request.py` & `LedgePythonSdk-0.0.2/test/test_create_quest_schedule_request.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_create_user_installed_games_request_inner.py` & `LedgePythonSdk-0.0.2/test/test_create_user_installed_games_request_inner.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_draw.py` & `LedgePythonSdk-0.0.2/test/test_draw.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_draw_api.py` & `LedgePythonSdk-0.0.2/test/test_draw_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_draw_detailed.py` & `LedgePythonSdk-0.0.2/test/test_draw_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_draw_product.py` & `LedgePythonSdk-0.0.2/test/test_draw_product.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_draw_product_detailed.py` & `LedgePythonSdk-0.0.2/test/test_draw_product_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_draw_schedule.py` & `LedgePythonSdk-0.0.2/test/test_draw_schedule.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_draw_schedule_detailed.py` & `LedgePythonSdk-0.0.2/test/test_draw_schedule_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_error_response.py` & `LedgePythonSdk-0.0.2/test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_external_activity.py` & `LedgePythonSdk-0.0.2/test/test_external_activity.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_external_api.py` & `LedgePythonSdk-0.0.2/test/test_external_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_external_user.py` & `LedgePythonSdk-0.0.2/test/test_external_user.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_game.py` & `LedgePythonSdk-0.0.2/test/test_game.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_game_detailed.py` & `LedgePythonSdk-0.0.2/test/test_game_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_game_genre.py` & `LedgePythonSdk-0.0.2/test/test_game_genre.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_game_genre_detailed.py` & `LedgePythonSdk-0.0.2/test/test_game_genre_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_game_images.py` & `LedgePythonSdk-0.0.2/test/test_game_images.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_game_tag.py` & `LedgePythonSdk-0.0.2/test/test_game_tag.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_game_tag_detailed.py` & `LedgePythonSdk-0.0.2/test/test_game_tag_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_game_with_title_icon.py` & `LedgePythonSdk-0.0.2/test/test_game_with_title_icon.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_games_api.py` & `LedgePythonSdk-0.0.2/test/test_games_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_gender.py` & `LedgePythonSdk-0.0.2/test/test_gender.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_genre.py` & `LedgePythonSdk-0.0.2/test/test_genre.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_genre_detailed.py` & `LedgePythonSdk-0.0.2/test/test_genre_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_get_profile200_response.py` & `LedgePythonSdk-0.0.2/test/test_get_profile200_response.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_goal.py` & `LedgePythonSdk-0.0.2/test/test_goal.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_goal_detailed.py` & `LedgePythonSdk-0.0.2/test/test_goal_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_goal_product.py` & `LedgePythonSdk-0.0.2/test/test_goal_product.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_goal_product_detailed.py` & `LedgePythonSdk-0.0.2/test/test_goal_product_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_guest_api.py` & `LedgePythonSdk-0.0.2/test/test_guest_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_inventory_api.py` & `LedgePythonSdk-0.0.2/test/test_inventory_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_leaderboard.py` & `LedgePythonSdk-0.0.2/test/test_leaderboard.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_leaderboard_api.py` & `LedgePythonSdk-0.0.2/test/test_leaderboard_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_listing.py` & `LedgePythonSdk-0.0.2/test/test_listing.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_listing_detailed.py` & `LedgePythonSdk-0.0.2/test/test_listing_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_listings_api.py` & `LedgePythonSdk-0.0.2/test/test_listings_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_merge_account_request.py` & `LedgePythonSdk-0.0.2/test/test_merge_account_request.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_notification.py` & `LedgePythonSdk-0.0.2/test/test_notification.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_notification_api.py` & `LedgePythonSdk-0.0.2/test/test_notification_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_notification_detailed.py` & `LedgePythonSdk-0.0.2/test/test_notification_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_notification_token.py` & `LedgePythonSdk-0.0.2/test/test_notification_token.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_notification_type.py` & `LedgePythonSdk-0.0.2/test/test_notification_type.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_paginated_case_reward_detailed.py` & `LedgePythonSdk-0.0.2/test/test_paginated_case_reward_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_paginated_case_reward_detailed_pagination.py` & `LedgePythonSdk-0.0.2/test/test_paginated_case_reward_detailed_pagination.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_paginated_game_detailed.py` & `LedgePythonSdk-0.0.2/test/test_paginated_game_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_paginated_listing_detailed.py` & `LedgePythonSdk-0.0.2/test/test_paginated_listing_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_paginated_notification_detailed.py` & `LedgePythonSdk-0.0.2/test/test_paginated_notification_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_paginated_quest_schedule_detailed.py` & `LedgePythonSdk-0.0.2/test/test_paginated_quest_schedule_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_paginated_rank_detailed.py` & `LedgePythonSdk-0.0.2/test/test_paginated_rank_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_paginated_screen_detailed.py` & `LedgePythonSdk-0.0.2/test/test_paginated_screen_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_paginated_transaction_detailed.py` & `LedgePythonSdk-0.0.2/test/test_paginated_transaction_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_period_type.py` & `LedgePythonSdk-0.0.2/test/test_period_type.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_player_stats.py` & `LedgePythonSdk-0.0.2/test/test_player_stats.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_processed_draw_schedule.py` & `LedgePythonSdk-0.0.2/test/test_processed_draw_schedule.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_product.py` & `LedgePythonSdk-0.0.2/test/test_product.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_product_api.py` & `LedgePythonSdk-0.0.2/test/test_product_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_product_swap.py` & `LedgePythonSdk-0.0.2/test/test_product_swap.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_product_type.py` & `LedgePythonSdk-0.0.2/test/test_product_type.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_progress.py` & `LedgePythonSdk-0.0.2/test/test_progress.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_quest.py` & `LedgePythonSdk-0.0.2/test/test_quest.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_quest_detailed.py` & `LedgePythonSdk-0.0.2/test/test_quest_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_quest_schedule.py` & `LedgePythonSdk-0.0.2/test/test_quest_schedule.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_quest_schedule_detailed.py` & `LedgePythonSdk-0.0.2/test/test_quest_schedule_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_quest_type.py` & `LedgePythonSdk-0.0.2/test/test_quest_type.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_quests_api.py` & `LedgePythonSdk-0.0.2/test/test_quests_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_rank.py` & `LedgePythonSdk-0.0.2/test/test_rank.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_rank_detailed.py` & `LedgePythonSdk-0.0.2/test/test_rank_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_register_request.py` & `LedgePythonSdk-0.0.2/test/test_register_request.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_screen.py` & `LedgePythonSdk-0.0.2/test/test_screen.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_screen_detailed.py` & `LedgePythonSdk-0.0.2/test/test_screen_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_screens_api.py` & `LedgePythonSdk-0.0.2/test/test_screens_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_social_api.py` & `LedgePythonSdk-0.0.2/test/test_social_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_social_profile.py` & `LedgePythonSdk-0.0.2/test/test_social_profile.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_status_type.py` & `LedgePythonSdk-0.0.2/test/test_status_type.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_tag.py` & `LedgePythonSdk-0.0.2/test/test_tag.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_tag_detailed.py` & `LedgePythonSdk-0.0.2/test/test_tag_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_track_activity200_response.py` & `LedgePythonSdk-0.0.2/test/test_track_activity200_response.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_transaction.py` & `LedgePythonSdk-0.0.2/test/test_transaction.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_transaction_api.py` & `LedgePythonSdk-0.0.2/test/test_transaction_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_transaction_detailed.py` & `LedgePythonSdk-0.0.2/test/test_transaction_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_transaction_type.py` & `LedgePythonSdk-0.0.2/test/test_transaction_type.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_update_notifications_request.py` & `LedgePythonSdk-0.0.2/test/test_update_notifications_request.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_update_profile_request.py` & `LedgePythonSdk-0.0.2/test/test_update_profile_request.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_update_request.py` & `LedgePythonSdk-0.0.2/test/test_update_request.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_user.py` & `LedgePythonSdk-0.0.2/test/test_user.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_user_api.py` & `LedgePythonSdk-0.0.2/test/test_user_api.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_user_connection.py` & `LedgePythonSdk-0.0.2/test/test_user_connection.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_user_draw.py` & `LedgePythonSdk-0.0.2/test/test_user_draw.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_user_draw_detailed.py` & `LedgePythonSdk-0.0.2/test/test_user_draw_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_user_inventory.py` & `LedgePythonSdk-0.0.2/test/test_user_inventory.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_user_inventory_detailed.py` & `LedgePythonSdk-0.0.2/test/test_user_inventory_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_user_quest_draw.py` & `LedgePythonSdk-0.0.2/test/test_user_quest_draw.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_user_quest_draw_detailed.py` & `LedgePythonSdk-0.0.2/test/test_user_quest_draw_detailed.py`

 * *Files identical despite different names*

### Comparing `LedgePythonSdk-0.0.1/test/test_user_spin_detailed.py` & `LedgePythonSdk-0.0.2/test/test_user_spin_detailed.py`

 * *Files identical despite different names*

