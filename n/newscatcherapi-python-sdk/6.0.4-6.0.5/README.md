# Comparing `tmp/newscatcherapi_python_sdk-6.0.4.tar.gz` & `tmp/newscatcherapi_python_sdk-6.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newscatcherapi_python_sdk-6.0.4.tar", max compression
+gzip compressed data, was "newscatcherapi_python_sdk-6.0.5.tar", max compression
```

## Comparing `newscatcherapi_python_sdk-6.0.4.tar` & `newscatcherapi_python_sdk-6.0.5.tar`

### file list

```diff
@@ -1,239 +1,259 @@
--rw-r--r--   0        0        0     1081 2024-04-19 17:40:04.230921 newscatcherapi_python_sdk-6.0.4/LICENSE
--rw-r--r--   0        0        0    75510 2024-04-19 17:53:34.550018 newscatcherapi_python_sdk-6.0.4/README.md
--rw-r--r--   0        0        0     1059 2024-04-19 17:53:34.550527 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/__init__.py
--rw-r--r--   0        0        0    77304 2024-04-19 17:53:34.550739 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/api_client.py
--rw-r--r--   0        0        0      663 2024-04-19 17:40:04.188946 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/api_response.py
--rw-r--r--   0        0        0      214 2024-04-19 17:40:04.189051 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/__init__.py
--rw-r--r--   0        0        0     1432 2024-04-19 17:40:04.189144 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/path_to_api.py
--rw-r--r--   0        0        0      248 2024-04-19 17:40:04.189238 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/paths/__init__.py
--rw-r--r--   0        0        0      197 2024-04-19 17:40:04.189332 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/paths/api_authors.py
--rw-r--r--   0        0        0      223 2024-04-19 17:40:04.189422 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/paths/api_latest_headlines.py
--rw-r--r--   0        0        0      194 2024-04-19 17:40:04.189513 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/paths/api_search.py
--rw-r--r--   0        0        0      216 2024-04-19 17:40:04.189603 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/paths/api_search_by_link.py
--rw-r--r--   0        0        0      217 2024-04-19 17:40:04.189689 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/paths/api_search_similar.py
--rw-r--r--   0        0        0      197 2024-04-19 17:40:04.189774 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/paths/api_sources.py
--rw-r--r--   0        0        0      212 2024-04-19 17:40:04.189860 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/paths/api_subscription.py
--rw-r--r--   0        0        0     1339 2024-04-19 17:40:04.189947 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tag_to_api.py
--rw-r--r--   0        0        0      507 2024-04-19 17:40:04.190038 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/__init__.py
--rw-r--r--   0        0        0      902 2024-04-19 17:40:04.190127 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/authors_api.py
--rw-r--r--   0        0        0      705 2024-04-19 17:40:04.190213 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/authors_api_raw.py
--rw-r--r--   0        0        0      961 2024-04-19 17:40:04.190302 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/latest_headlines_api.py
--rw-r--r--   0        0        0      731 2024-04-19 17:40:04.190396 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/latest_headlines_api_raw.py
--rw-r--r--   0        0        0      895 2024-04-19 17:40:04.190488 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/search_api.py
--rw-r--r--   0        0        0      702 2024-04-19 17:40:04.190574 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/search_api_raw.py
--rw-r--r--   0        0        0      932 2024-04-19 17:40:04.190662 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/search_link_api.py
--rw-r--r--   0        0        0      722 2024-04-19 17:40:04.190759 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/search_link_api_raw.py
--rw-r--r--   0        0        0      947 2024-04-19 17:40:04.191017 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/search_similar_api.py
--rw-r--r--   0        0        0      725 2024-04-19 17:40:04.191118 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/search_similar_api_raw.py
--rw-r--r--   0        0        0      902 2024-04-19 17:40:04.191214 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/sources_api.py
--rw-r--r--   0        0        0      705 2024-04-19 17:40:04.191312 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/sources_api_raw.py
--rw-r--r--   0        0        0      937 2024-04-19 17:40:04.191418 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/subscription_api.py
--rw-r--r--   0        0        0      720 2024-04-19 17:40:04.191515 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/subscription_api_raw.py
--rw-r--r--   0        0        0     2114 2024-04-19 17:40:04.191614 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/client.py
--rw-r--r--   0        0        0     2114 2024-04-19 17:40:04.191708 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/client.pyi
--rw-r--r--   0        0        0      950 2024-04-19 17:40:04.191800 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/client_custom.py
--rw-r--r--   0        0        0    18272 2024-04-19 17:53:34.550892 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/configuration.py
--rw-r--r--   0        0        0     7953 2024-04-19 17:40:04.192038 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/exceptions.py
--rw-r--r--   0        0        0     2274 2024-04-19 17:40:04.192134 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/exceptions_base.py
--rw-r--r--   0        0        0      355 2024-04-19 17:40:04.192269 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/__init__.py
--rw-r--r--   0        0        0     3784 2024-04-19 17:53:34.551018 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/additional_source_info.py
--rw-r--r--   0        0        0     3784 2024-04-19 17:53:34.551120 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/additional_source_info.pyi
--rw-r--r--   0        0        0    31500 2024-04-19 17:53:34.551253 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/author_search_request.py
--rw-r--r--   0        0        0    31184 2024-04-19 17:53:34.551385 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/author_search_request.pyi
--rw-r--r--   0        0        0     2575 2024-04-19 17:40:04.192995 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/authors_get_response.py
--rw-r--r--   0        0        0     2575 2024-04-19 17:40:04.193195 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/authors_get_response.pyi
--rw-r--r--   0        0        0     2577 2024-04-19 17:40:04.193606 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/authors_post_response.py
--rw-r--r--   0        0        0     2577 2024-04-19 17:40:04.193821 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/authors_post_response.pyi
--rw-r--r--   0        0        0     3926 2024-04-19 17:53:34.551510 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/cluster.py
--rw-r--r--   0        0        0     3926 2024-04-19 17:53:34.551640 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/cluster.pyi
--rw-r--r--   0        0        0     1483 2024-04-19 17:40:04.194616 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/cluster_articles.py
--rw-r--r--   0        0        0     1483 2024-04-19 17:40:04.195127 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/cluster_articles.pyi
--rw-r--r--   0        0        0     7607 2024-04-19 17:53:34.551759 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/clustering_search_response.py
--rw-r--r--   0        0        0     7607 2024-04-19 17:53:34.551864 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/clustering_search_response.pyi
--rw-r--r--   0        0        0    31387 2024-04-19 17:53:34.552013 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_article_result.py
--rw-r--r--   0        0        0    31387 2024-04-19 17:53:34.552136 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_article_result.pyi
--rw-r--r--   0        0        0     7229 2024-04-19 17:53:34.552268 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.py
--rw-r--r--   0        0        0     7229 2024-04-19 17:53:34.552403 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.pyi
--rw-r--r--   0        0        0     6499 2024-04-19 17:53:34.552527 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_search_response.py
--rw-r--r--   0        0        0     6499 2024-04-19 17:53:34.552640 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_search_response.pyi
--rw-r--r--   0        0        0     1561 2024-04-19 17:40:04.198114 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.py
--rw-r--r--   0        0        0     1561 2024-04-19 17:40:04.198247 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.pyi
--rw-r--r--   0        0        0    33012 2024-04-19 17:53:34.552766 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.py
--rw-r--r--   0        0        0    33012 2024-04-19 17:53:34.553052 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.pyi
--rw-r--r--   0        0        0     7228 2024-04-19 17:53:34.553181 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.py
--rw-r--r--   0        0        0     7228 2024-04-19 17:53:34.553301 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.pyi
--rw-r--r--   0        0        0     6499 2024-04-19 17:53:34.553419 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.py
--rw-r--r--   0        0        0     6499 2024-04-19 17:53:34.553529 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.pyi
--rw-r--r--   0        0        0     1561 2024-04-19 17:40:04.199081 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.py
--rw-r--r--   0        0        0     1561 2024-04-19 17:40:04.199176 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.pyi
--rw-r--r--   0        0        0     6437 2024-04-19 17:53:34.553634 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_search_response_search_response.py
--rw-r--r--   0        0        0     6437 2024-04-19 17:53:34.553734 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_search_response_search_response.pyi
--rw-r--r--   0        0        0     1549 2024-04-19 17:40:04.200663 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.py
--rw-r--r--   0        0        0     1549 2024-04-19 17:40:04.201373 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.pyi
--rw-r--r--   0        0        0     3525 2024-04-19 17:40:04.202603 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/http_validation_error.py
--rw-r--r--   0        0        0     3525 2024-04-19 17:40:04.203006 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/http_validation_error.pyi
--rw-r--r--   0        0        0     2429 2024-04-19 17:40:04.203802 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_get_response.py
--rw-r--r--   0        0        0     2429 2024-04-19 17:40:04.204002 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_get_response.pyi
--rw-r--r--   0        0        0     2431 2024-04-19 17:40:04.205533 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_post_response.py
--rw-r--r--   0        0        0     2431 2024-04-19 17:40:04.205813 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_post_response.pyi
--rw-r--r--   0        0        0    28271 2024-04-19 17:53:34.553852 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_request.py
--rw-r--r--   0        0        0    27955 2024-04-19 17:53:34.553982 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_request.pyi
--rw-r--r--   0        0        0     6273 2024-04-19 17:53:34.554213 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_response.py
--rw-r--r--   0        0        0     6273 2024-04-19 17:53:34.554310 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_response.pyi
--rw-r--r--   0        0        0     1515 2024-04-19 17:40:04.206400 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_response_articles.py
--rw-r--r--   0        0        0     1515 2024-04-19 17:40:04.206501 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_response_articles.pyi
--rw-r--r--   0        0        0    32258 2024-04-19 17:53:34.554432 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/more_like_this_request.py
--rw-r--r--   0        0        0    31863 2024-04-19 17:53:34.554559 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/more_like_this_request.pyi
--rw-r--r--   0        0        0     2465 2024-04-19 17:40:04.206847 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_get_response.py
--rw-r--r--   0        0        0     2465 2024-04-19 17:40:04.206937 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_get_response.pyi
--rw-r--r--   0        0        0     2467 2024-04-19 17:40:04.207028 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_post_response.py
--rw-r--r--   0        0        0     2467 2024-04-19 17:40:04.207123 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_post_response.pyi
--rw-r--r--   0        0        0    36757 2024-04-19 17:53:34.554689 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_request.py
--rw-r--r--   0        0        0    36441 2024-04-19 17:53:34.554831 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_request.pyi
--rw-r--r--   0        0        0     2589 2024-04-19 17:40:04.207461 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_similar_get_response.py
--rw-r--r--   0        0        0     2589 2024-04-19 17:40:04.207554 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_similar_get_response.pyi
--rw-r--r--   0        0        0     2591 2024-04-19 17:40:04.207642 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_similar_post_response.py
--rw-r--r--   0        0        0     2591 2024-04-19 17:40:04.207765 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_similar_post_response.pyi
--rw-r--r--   0        0        0     4717 2024-04-19 17:53:34.554953 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_url_request.py
--rw-r--r--   0        0        0     4559 2024-04-19 17:53:34.555058 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_url_request.pyi
--rw-r--r--   0        0        0     4044 2024-04-19 17:53:34.555160 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/similar_document.py
--rw-r--r--   0        0        0     4044 2024-04-19 17:53:34.555261 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/similar_document.pyi
--rw-r--r--   0        0        0     4488 2024-04-19 17:53:34.555374 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/source_info.py
--rw-r--r--   0        0        0     4488 2024-04-19 17:53:34.555471 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/source_info.pyi
--rw-r--r--   0        0        0     3912 2024-04-19 17:53:34.555575 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/source_response.py
--rw-r--r--   0        0        0     3912 2024-04-19 17:53:34.555667 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/source_response.pyi
--rw-r--r--   0        0        0     3437 2024-04-19 17:40:04.208700 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/source_response_sources.py
--rw-r--r--   0        0        0     3437 2024-04-19 17:40:04.208800 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/source_response_sources.pyi
--rw-r--r--   0        0        0     6854 2024-04-19 17:53:34.555778 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/sources_request.py
--rw-r--r--   0        0        0     6854 2024-04-19 17:53:34.555874 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/sources_request.pyi
--rw-r--r--   0        0        0     5919 2024-04-19 17:53:34.555978 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/subscription_response.py
--rw-r--r--   0        0        0     5919 2024-04-19 17:53:34.556077 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/subscription_response.pyi
--rw-r--r--   0        0        0     3626 2024-04-19 17:40:04.209362 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/validation_error.py
--rw-r--r--   0        0        0     3626 2024-04-19 17:40:04.209457 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/validation_error.pyi
--rw-r--r--   0        0        0     3408 2024-04-19 17:40:04.209553 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/validation_error_loc.py
--rw-r--r--   0        0        0     3408 2024-04-19 17:40:04.209653 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/validation_error_loc.pyi
--rw-r--r--   0        0        0     4137 2024-04-19 17:40:04.209761 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/models/__init__.py
--rw-r--r--   0        0        0    25039 2024-04-19 17:53:34.556234 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/operation_parameter_map.py
--rw-r--r--   0        0        0      582 2024-04-19 17:40:04.210000 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/__init__.py
--rw-r--r--   0        0        0      323 2024-04-19 17:40:04.210101 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_authors/__init__.py
--rw-r--r--   0        0        0    66916 2024-04-19 17:53:34.556468 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_authors/get.py
--rw-r--r--   0        0        0    66607 2024-04-19 17:53:34.557062 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_authors/get.pyi
--rw-r--r--   0        0        0    47473 2024-04-19 17:53:34.557217 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_authors/post.py
--rw-r--r--   0        0        0    47336 2024-04-19 17:53:34.557365 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_authors/post.pyi
--rw-r--r--   0        0        0      341 2024-04-19 17:40:04.210787 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_latest_headlines/__init__.py
--rw-r--r--   0        0        0    66032 2024-04-19 17:53:34.557727 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_latest_headlines/get.py
--rw-r--r--   0        0        0    65723 2024-04-19 17:53:34.557902 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_latest_headlines/get.pyi
--rw-r--r--   0        0        0    49192 2024-04-19 17:53:34.558070 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_latest_headlines/post.py
--rw-r--r--   0        0        0    49055 2024-04-19 17:53:34.558264 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_latest_headlines/post.pyi
--rw-r--r--   0        0        0      321 2024-04-19 17:40:04.211502 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search/__init__.py
--rw-r--r--   0        0        0    77343 2024-04-19 17:53:34.558463 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search/get.py
--rw-r--r--   0        0        0    77034 2024-04-19 17:53:34.558675 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search/get.pyi
--rw-r--r--   0        0        0    54404 2024-04-19 17:53:34.558843 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search/post.py
--rw-r--r--   0        0        0    54267 2024-04-19 17:53:34.559013 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search/post.pyi
--rw-r--r--   0        0        0      337 2024-04-19 17:40:04.212230 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_by_link/__init__.py
--rw-r--r--   0        0        0    19293 2024-04-19 17:40:04.212336 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_by_link/get.py
--rw-r--r--   0        0        0    19070 2024-04-19 17:40:04.212460 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_by_link/get.pyi
--rw-r--r--   0        0        0    17699 2024-04-19 17:40:04.212610 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_by_link/post.py
--rw-r--r--   0        0        0    17562 2024-04-19 17:40:04.212731 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_by_link/post.pyi
--rw-r--r--   0        0        0      337 2024-04-19 17:40:04.212849 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_similar/__init__.py
--rw-r--r--   0        0        0    67713 2024-04-19 17:40:04.212991 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_similar/get.py
--rw-r--r--   0        0        0    67361 2024-04-19 17:40:04.213152 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_similar/get.pyi
--rw-r--r--   0        0        0    47930 2024-04-19 17:40:04.213293 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_similar/post.py
--rw-r--r--   0        0        0    47793 2024-04-19 17:40:04.213423 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_similar/post.pyi
--rw-r--r--   0        0        0      323 2024-04-19 17:40:04.213538 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_sources/__init__.py
--rw-r--r--   0        0        0    22889 2024-04-19 17:40:04.213643 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_sources/get.py
--rw-r--r--   0        0        0    22752 2024-04-19 17:40:04.213786 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_sources/get.pyi
--rw-r--r--   0        0        0    19936 2024-04-19 17:40:04.214231 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_sources/post.py
--rw-r--r--   0        0        0    19799 2024-04-19 17:40:04.214365 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_sources/post.pyi
--rw-r--r--   0        0        0      333 2024-04-19 17:40:04.214491 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_subscription/__init__.py
--rw-r--r--   0        0        0    12067 2024-04-19 17:40:04.214601 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_subscription/get.py
--rw-r--r--   0        0        0    11930 2024-04-19 17:40:04.214745 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_subscription/get.pyi
--rw-r--r--   0        0        0    12093 2024-04-19 17:40:04.214878 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_subscription/post.py
--rw-r--r--   0        0        0    11956 2024-04-19 17:40:04.215531 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_subscription/post.pyi
--rw-r--r--   0        0        0        0 2024-04-19 17:40:04.215957 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/__init__.py
--rw-r--r--   0        0        0      987 2024-04-19 17:40:04.216048 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/additional_source_info.py
--rw-r--r--   0        0        0     4726 2024-04-19 17:53:34.559173 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/author_search_request.py
--rw-r--r--   0        0        0     1061 2024-04-19 17:40:04.216235 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/authors_get_response.py
--rw-r--r--   0        0        0     1062 2024-04-19 17:40:04.216330 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/authors_post_response.py
--rw-r--r--   0        0        0      995 2024-04-19 17:40:04.216415 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/cluster.py
--rw-r--r--   0        0        0      665 2024-04-19 17:40:04.216499 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/cluster_articles.py
--rw-r--r--   0        0        0     1336 2024-04-19 17:40:04.216592 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/clustering_search_response.py
--rw-r--r--   0        0        0     3052 2024-04-19 17:40:04.216694 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_author_search_response_article_result.py
--rw-r--r--   0        0        0     1542 2024-04-19 17:40:04.216809 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_author_search_response_failed_search_response.py
--rw-r--r--   0        0        0     1436 2024-04-19 17:40:04.216907 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response.py
--rw-r--r--   0        0        0      704 2024-04-19 17:40:04.217000 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response_articles.py
--rw-r--r--   0        0        0     3239 2024-04-19 17:40:04.217091 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_article_result.py
--rw-r--r--   0        0        0     1543 2024-04-19 17:40:04.217184 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_failed_search_response.py
--rw-r--r--   0        0        0     1437 2024-04-19 17:40:04.217278 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response.py
--rw-r--r--   0        0        0      704 2024-04-19 17:40:04.217372 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response_articles.py
--rw-r--r--   0        0        0     1411 2024-04-19 17:40:04.217462 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_search_response_search_response.py
--rw-r--r--   0        0        0      698 2024-04-19 17:40:04.217553 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_search_response_search_response_articles.py
--rw-r--r--   0        0        0      937 2024-04-19 17:40:04.217648 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/http_validation_error.py
--rw-r--r--   0        0        0      907 2024-04-19 17:40:04.217740 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/latest_headlines_get_response.py
--rw-r--r--   0        0        0      908 2024-04-19 17:40:04.217825 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/latest_headlines_post_response.py
--rw-r--r--   0        0        0     4897 2024-04-19 17:53:34.559286 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/latest_headlines_request.py
--rw-r--r--   0        0        0     1340 2024-04-19 17:40:04.218013 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/latest_headlines_response.py
--rw-r--r--   0        0        0      681 2024-04-19 17:40:04.218099 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/latest_headlines_response_articles.py
--rw-r--r--   0        0        0     4721 2024-04-19 17:40:04.218191 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/more_like_this_request.py
--rw-r--r--   0        0        0      952 2024-04-19 17:40:04.218275 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/search_get_response.py
--rw-r--r--   0        0        0      953 2024-04-19 17:40:04.218368 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/search_post_response.py
--rw-r--r--   0        0        0     5539 2024-04-19 17:53:34.559396 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/search_request.py
--rw-r--r--   0        0        0     1069 2024-04-19 17:40:04.218549 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/search_similar_get_response.py
--rw-r--r--   0        0        0     1070 2024-04-19 17:40:04.218635 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/search_similar_post_response.py
--rw-r--r--   0        0        0     1151 2024-04-19 17:40:04.218724 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/search_url_request.py
--rw-r--r--   0        0        0      937 2024-04-19 17:40:04.218812 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/similar_document.py
--rw-r--r--   0        0        0     1132 2024-04-19 17:40:04.218895 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/source_info.py
--rw-r--r--   0        0        0     1093 2024-04-19 17:40:04.218981 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/source_response.py
--rw-r--r--   0        0        0      760 2024-04-19 17:40:04.219074 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/source_response_sources.py
--rw-r--r--   0        0        0     1432 2024-04-19 17:40:04.219159 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/sources_request.py
--rw-r--r--   0        0        0     1216 2024-04-19 17:40:04.219243 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/subscription_response.py
--rw-r--r--   0        0        0      973 2024-04-19 17:40:04.219330 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/validation_error.py
--rw-r--r--   0        0        0      684 2024-04-19 17:40:04.219432 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/validation_error_loc.py
--rw-r--r--   0        0        0      913 2024-04-19 17:40:04.219528 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/request_after_hook.py
--rw-r--r--   0        0        0      971 2024-04-19 17:40:04.219616 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/request_before_hook.py
--rw-r--r--   0        0        0      936 2024-04-19 17:40:04.219710 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/request_before_url_hook.py
--rw-r--r--   0        0        0    11233 2024-04-19 17:40:04.219818 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/rest.py
--rw-r--r--   0        0        0    96391 2024-04-19 17:40:04.220036 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/schemas.py
--rw-r--r--   0        0        0        0 2024-04-19 17:40:04.220150 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/__init__.py
--rw-r--r--   0        0        0      842 2024-04-19 17:40:04.220245 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/additional_source_info.py
--rw-r--r--   0        0        0     2699 2024-04-19 17:53:34.559523 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/author_search_request.py
--rw-r--r--   0        0        0      992 2024-04-19 17:40:04.220450 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/authors_get_response.py
--rw-r--r--   0        0        0      993 2024-04-19 17:40:04.220582 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/authors_post_response.py
--rw-r--r--   0        0        0      862 2024-04-19 17:40:04.220720 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/cluster.py
--rw-r--r--   0        0        0      604 2024-04-19 17:40:04.220873 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/cluster_articles.py
--rw-r--r--   0        0        0     1106 2024-04-19 17:40:04.221004 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/clustering_search_response.py
--rw-r--r--   0        0        0     1778 2024-04-19 17:40:04.221103 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_author_search_response_article_result.py
--rw-r--r--   0        0        0     1341 2024-04-19 17:40:04.221202 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_author_search_response_failed_search_response.py
--rw-r--r--   0        0        0     1326 2024-04-19 17:40:04.221302 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_author_search_response_search_response.py
--rw-r--r--   0        0        0      643 2024-04-19 17:40:04.221400 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_author_search_response_search_response_articles.py
--rw-r--r--   0        0        0     1903 2024-04-19 17:40:04.221494 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_more_like_this_response_article_result.py
--rw-r--r--   0        0        0     1342 2024-04-19 17:40:04.221596 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_more_like_this_response_failed_search_response.py
--rw-r--r--   0        0        0     1327 2024-04-19 17:40:04.221690 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response.py
--rw-r--r--   0        0        0      643 2024-04-19 17:40:04.221790 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response_articles.py
--rw-r--r--   0        0        0     1277 2024-04-19 17:40:04.221884 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_search_response_search_response.py
--rw-r--r--   0        0        0      637 2024-04-19 17:40:04.221980 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_search_response_search_response_articles.py
--rw-r--r--   0        0        0      889 2024-04-19 17:40:04.222070 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/http_validation_error.py
--rw-r--r--   0        0        0      838 2024-04-19 17:40:04.222159 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/latest_headlines_get_response.py
--rw-r--r--   0        0        0      839 2024-04-19 17:40:04.222247 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/latest_headlines_post_response.py
--rw-r--r--   0        0        0     2812 2024-04-19 17:53:34.559640 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/latest_headlines_request.py
--rw-r--r--   0        0        0     1138 2024-04-19 17:40:04.222498 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/latest_headlines_response.py
--rw-r--r--   0        0        0      620 2024-04-19 17:40:04.222605 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/latest_headlines_response_articles.py
--rw-r--r--   0        0        0     2616 2024-04-19 17:40:04.222814 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/more_like_this_request.py
--rw-r--r--   0        0        0      883 2024-04-19 17:40:04.222912 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/search_get_response.py
--rw-r--r--   0        0        0      884 2024-04-19 17:40:04.223013 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/search_post_response.py
--rw-r--r--   0        0        0     3031 2024-04-19 17:53:34.559747 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/search_request.py
--rw-r--r--   0        0        0     1000 2024-04-19 17:40:04.223198 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/search_similar_get_response.py
--rw-r--r--   0        0        0     1001 2024-04-19 17:40:04.223427 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/search_similar_post_response.py
--rw-r--r--   0        0        0      957 2024-04-19 17:40:04.223520 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/search_url_request.py
--rw-r--r--   0        0        0      836 2024-04-19 17:40:04.223627 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/similar_document.py
--rw-r--r--   0        0        0      904 2024-04-19 17:40:04.223710 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/source_info.py
--rw-r--r--   0        0        0      994 2024-04-19 17:40:04.223795 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/source_response.py
--rw-r--r--   0        0        0      695 2024-04-19 17:40:04.223883 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/source_response_sources.py
--rw-r--r--   0        0        0      996 2024-04-19 17:40:04.223964 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/sources_request.py
--rw-r--r--   0        0        0      925 2024-04-19 17:40:04.224045 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/subscription_response.py
--rw-r--r--   0        0        0      892 2024-04-19 17:40:04.224127 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/validation_error.py
--rw-r--r--   0        0        0      623 2024-04-19 17:40:04.224211 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/validation_error_loc.py
--rw-r--r--   0        0        0      758 2024-04-19 17:40:04.224296 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type_util.py
--rw-r--r--   0        0        0     3177 2024-04-19 17:40:04.224385 newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/validation_metadata.py
--rw-r--r--   0        0        0      791 2024-04-19 17:53:34.559852 newscatcherapi_python_sdk-6.0.4/pyproject.toml
--rw-r--r--   0        0        0    76527 1970-01-01 00:00:00.000000 newscatcherapi_python_sdk-6.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-25 19:58:24.285935 newscatcherapi_python_sdk-6.0.5/LICENSE
+-rw-r--r--   0        0        0    77971 2024-04-25 20:02:27.020398 newscatcherapi_python_sdk-6.0.5/README.md
+-rw-r--r--   0        0        0     1059 2024-04-25 20:02:27.020547 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/__init__.py
+-rw-r--r--   0        0        0    77304 2024-04-25 20:02:27.020779 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/api_client.py
+-rw-r--r--   0        0        0      663 2024-04-25 19:58:24.246592 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/api_response.py
+-rw-r--r--   0        0        0      214 2024-04-25 19:58:24.246713 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/__init__.py
+-rw-r--r--   0        0        0     1726 2024-04-25 20:02:27.020942 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/path_to_api.py
+-rw-r--r--   0        0        0      248 2024-04-25 19:58:24.246991 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/paths/__init__.py
+-rw-r--r--   0        0        0      197 2024-04-25 19:58:24.247093 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/paths/api_authors.py
+-rw-r--r--   0        0        0      223 2024-04-25 19:58:24.247196 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/paths/api_latest_headlines.py
+-rw-r--r--   0        0        0      194 2024-04-25 19:58:24.247290 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/paths/api_search.py
+-rw-r--r--   0        0        0      216 2024-04-25 19:58:24.247381 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/paths/api_search_by_link.py
+-rw-r--r--   0        0        0      268 2024-04-25 20:02:27.021036 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/paths/api_search_duplicates_by_original_id.py
+-rw-r--r--   0        0        0      217 2024-04-25 19:58:24.247682 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/paths/api_search_similar.py
+-rw-r--r--   0        0        0      197 2024-04-25 19:58:24.247771 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/paths/api_sources.py
+-rw-r--r--   0        0        0      212 2024-04-25 19:58:24.247858 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/paths/api_subscription.py
+-rw-r--r--   0        0        0     1622 2024-04-25 20:02:27.021176 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tag_to_api.py
+-rw-r--r--   0        0        0      581 2024-04-25 20:02:27.021334 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/__init__.py
+-rw-r--r--   0        0        0      902 2024-04-25 19:58:24.248147 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/authors_api.py
+-rw-r--r--   0        0        0      705 2024-04-25 19:58:24.248252 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/authors_api_raw.py
+-rw-r--r--   0        0        0      961 2024-04-25 19:58:24.248403 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/latest_headlines_api.py
+-rw-r--r--   0        0        0      731 2024-04-25 19:58:24.248544 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/latest_headlines_api_raw.py
+-rw-r--r--   0        0        0      895 2024-04-25 19:58:24.248659 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_api.py
+-rw-r--r--   0        0        0      702 2024-04-25 19:58:24.248773 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_api_raw.py
+-rw-r--r--   0        0        0     1061 2024-04-25 20:02:27.021453 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_duplicates_by_original_id_api.py
+-rw-r--r--   0        0        0      776 2024-04-25 20:02:27.021592 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_duplicates_by_original_id_api_raw.py
+-rw-r--r--   0        0        0      932 2024-04-25 19:58:24.249098 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_link_api.py
+-rw-r--r--   0        0        0      722 2024-04-25 19:58:24.249203 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_link_api_raw.py
+-rw-r--r--   0        0        0      947 2024-04-25 19:58:24.249303 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_similar_api.py
+-rw-r--r--   0        0        0      725 2024-04-25 19:58:24.249436 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_similar_api_raw.py
+-rw-r--r--   0        0        0      902 2024-04-25 19:58:24.249554 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/sources_api.py
+-rw-r--r--   0        0        0      705 2024-04-25 19:58:24.249662 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/sources_api_raw.py
+-rw-r--r--   0        0        0      937 2024-04-25 19:58:24.249876 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/subscription_api.py
+-rw-r--r--   0        0        0      720 2024-04-25 19:58:24.249975 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/subscription_api_raw.py
+-rw-r--r--   0        0        0     2352 2024-04-25 20:02:27.021756 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/client.py
+-rw-r--r--   0        0        0     2352 2024-04-25 20:02:27.021919 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/client.pyi
+-rw-r--r--   0        0        0      950 2024-04-25 19:58:24.250278 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/client_custom.py
+-rw-r--r--   0        0        0    18272 2024-04-25 20:02:27.022098 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/configuration.py
+-rw-r--r--   0        0        0     7953 2024-04-25 19:58:24.250519 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/exceptions.py
+-rw-r--r--   0        0        0     2274 2024-04-25 19:58:24.250625 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/exceptions_base.py
+-rw-r--r--   0        0        0      355 2024-04-25 19:58:24.250761 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/__init__.py
+-rw-r--r--   0        0        0     3784 2024-04-25 19:58:24.250862 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/additional_source_info.py
+-rw-r--r--   0        0        0     3784 2024-04-25 19:58:24.250958 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/additional_source_info.pyi
+-rw-r--r--   0        0        0    31500 2024-04-25 19:58:24.251067 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/author_search_request.py
+-rw-r--r--   0        0        0    31184 2024-04-25 19:58:24.251196 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/author_search_request.pyi
+-rw-r--r--   0        0        0     2575 2024-04-25 19:58:24.251304 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/authors_get_response.py
+-rw-r--r--   0        0        0     2575 2024-04-25 19:58:24.251406 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/authors_get_response.pyi
+-rw-r--r--   0        0        0     2577 2024-04-25 19:58:24.251515 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/authors_post_response.py
+-rw-r--r--   0        0        0     2577 2024-04-25 19:58:24.251616 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/authors_post_response.pyi
+-rw-r--r--   0        0        0     3926 2024-04-25 19:58:24.251719 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/cluster.py
+-rw-r--r--   0        0        0     3926 2024-04-25 19:58:24.251816 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/cluster.pyi
+-rw-r--r--   0        0        0     1483 2024-04-25 19:58:24.251924 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/cluster_articles.py
+-rw-r--r--   0        0        0     1483 2024-04-25 19:58:24.252144 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/cluster_articles.pyi
+-rw-r--r--   0        0        0     7607 2024-04-25 19:58:24.252273 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/clustering_search_response.py
+-rw-r--r--   0        0        0     7607 2024-04-25 19:58:24.252422 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/clustering_search_response.pyi
+-rw-r--r--   0        0        0    31387 2024-04-25 19:58:24.252555 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_article_result.py
+-rw-r--r--   0        0        0    31387 2024-04-25 19:58:24.252697 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_article_result.pyi
+-rw-r--r--   0        0        0     7229 2024-04-25 19:58:24.252840 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.py
+-rw-r--r--   0        0        0     7229 2024-04-25 19:58:24.252968 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.pyi
+-rw-r--r--   0        0        0     6499 2024-04-25 19:58:24.253093 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_search_response.py
+-rw-r--r--   0        0        0     6499 2024-04-25 19:58:24.253221 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_search_response.pyi
+-rw-r--r--   0        0        0     1561 2024-04-25 19:58:24.253332 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.py
+-rw-r--r--   0        0        0     1561 2024-04-25 19:58:24.253442 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.pyi
+-rw-r--r--   0        0        0    33012 2024-04-25 19:58:24.253562 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.py
+-rw-r--r--   0        0        0    33012 2024-04-25 19:58:24.253717 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.pyi
+-rw-r--r--   0        0        0     7228 2024-04-25 19:58:24.253853 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.py
+-rw-r--r--   0        0        0     7228 2024-04-25 19:58:24.253974 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.pyi
+-rw-r--r--   0        0        0     6499 2024-04-25 19:58:24.254093 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.py
+-rw-r--r--   0        0        0     6499 2024-04-25 19:58:24.254215 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.pyi
+-rw-r--r--   0        0        0     1561 2024-04-25 19:58:24.254329 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.py
+-rw-r--r--   0        0        0     1561 2024-04-25 19:58:24.254443 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.pyi
+-rw-r--r--   0        0        0     6437 2024-04-25 19:58:24.254566 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_search_response_search_response.py
+-rw-r--r--   0        0        0     6437 2024-04-25 19:58:24.254682 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_search_response_search_response.pyi
+-rw-r--r--   0        0        0     1549 2024-04-25 19:58:24.254799 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.py
+-rw-r--r--   0        0        0     1549 2024-04-25 19:58:24.254904 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.pyi
+-rw-r--r--   0        0        0     4257 2024-04-25 20:02:27.022250 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/duplicates_by_original_id_request.py
+-rw-r--r--   0        0        0     4099 2024-04-25 20:02:27.022444 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/duplicates_by_original_id_request.pyi
+-rw-r--r--   0        0        0     3525 2024-04-25 19:58:24.255225 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/http_validation_error.py
+-rw-r--r--   0        0        0     3525 2024-04-25 19:58:24.255311 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/http_validation_error.pyi
+-rw-r--r--   0        0        0     2429 2024-04-25 19:58:24.255401 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_get_response.py
+-rw-r--r--   0        0        0     2429 2024-04-25 19:58:24.255492 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_get_response.pyi
+-rw-r--r--   0        0        0     2431 2024-04-25 19:58:24.255581 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_post_response.py
+-rw-r--r--   0        0        0     2431 2024-04-25 19:58:24.256025 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_post_response.pyi
+-rw-r--r--   0        0        0    28271 2024-04-25 19:58:24.256168 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_request.py
+-rw-r--r--   0        0        0    27955 2024-04-25 19:58:24.256293 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_request.pyi
+-rw-r--r--   0        0        0     6273 2024-04-25 19:58:24.256415 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_response.py
+-rw-r--r--   0        0        0     6273 2024-04-25 19:58:24.256526 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_response.pyi
+-rw-r--r--   0        0        0     1515 2024-04-25 19:58:24.256621 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_response_articles.py
+-rw-r--r--   0        0        0     1515 2024-04-25 19:58:24.256719 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_response_articles.pyi
+-rw-r--r--   0        0        0    32258 2024-04-25 19:58:24.256821 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/more_like_this_request.py
+-rw-r--r--   0        0        0    31863 2024-04-25 19:58:24.256942 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/more_like_this_request.pyi
+-rw-r--r--   0        0        0     2465 2024-04-25 19:58:24.257043 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_get_response.py
+-rw-r--r--   0        0        0     2465 2024-04-25 19:58:24.257130 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_get_response.pyi
+-rw-r--r--   0        0        0     2467 2024-04-25 19:58:24.257215 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_post_response.py
+-rw-r--r--   0        0        0     2467 2024-04-25 19:58:24.257305 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_post_response.pyi
+-rw-r--r--   0        0        0    37420 2024-04-25 20:02:27.022823 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_request.py
+-rw-r--r--   0        0        0    37104 2024-04-25 20:02:27.022977 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_request.pyi
+-rw-r--r--   0        0        0     2589 2024-04-25 19:58:24.257625 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_similar_get_response.py
+-rw-r--r--   0        0        0     2589 2024-04-25 19:58:24.257712 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_similar_get_response.pyi
+-rw-r--r--   0        0        0     2591 2024-04-25 19:58:24.257799 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_similar_post_response.py
+-rw-r--r--   0        0        0     2591 2024-04-25 19:58:24.257889 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_similar_post_response.pyi
+-rw-r--r--   0        0        0     4717 2024-04-25 19:58:24.257991 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_url_request.py
+-rw-r--r--   0        0        0     4559 2024-04-25 19:58:24.258092 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_url_request.pyi
+-rw-r--r--   0        0        0     2509 2024-04-25 20:02:27.023102 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/searchduplicatesbyoriginalid_get_response.py
+-rw-r--r--   0        0        0     2509 2024-04-25 20:02:27.023180 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/searchduplicatesbyoriginalid_get_response.pyi
+-rw-r--r--   0        0        0     2511 2024-04-25 20:02:27.023247 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/searchduplicatesbyoriginalid_post_response.py
+-rw-r--r--   0        0        0     2511 2024-04-25 20:02:27.023311 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/searchduplicatesbyoriginalid_post_response.pyi
+-rw-r--r--   0        0        0     4044 2024-04-25 19:58:24.258708 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/similar_document.py
+-rw-r--r--   0        0        0     4044 2024-04-25 19:58:24.258802 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/similar_document.pyi
+-rw-r--r--   0        0        0     4488 2024-04-25 19:58:24.258904 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/source_info.py
+-rw-r--r--   0        0        0     4488 2024-04-25 19:58:24.259005 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/source_info.pyi
+-rw-r--r--   0        0        0     3912 2024-04-25 19:58:24.259100 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/source_response.py
+-rw-r--r--   0        0        0     3912 2024-04-25 19:58:24.259191 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/source_response.pyi
+-rw-r--r--   0        0        0     3437 2024-04-25 19:58:24.259279 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/source_response_sources.py
+-rw-r--r--   0        0        0     3437 2024-04-25 19:58:24.259365 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/source_response_sources.pyi
+-rw-r--r--   0        0        0     6854 2024-04-25 19:58:24.259461 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/sources_request.py
+-rw-r--r--   0        0        0     6854 2024-04-25 19:58:24.259556 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/sources_request.pyi
+-rw-r--r--   0        0        0     5919 2024-04-25 19:58:24.259659 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/subscription_response.py
+-rw-r--r--   0        0        0     5919 2024-04-25 19:58:24.259756 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/subscription_response.pyi
+-rw-r--r--   0        0        0     3626 2024-04-25 19:58:24.259953 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/validation_error.py
+-rw-r--r--   0        0        0     3626 2024-04-25 19:58:24.260036 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/validation_error.pyi
+-rw-r--r--   0        0        0     3408 2024-04-25 19:58:24.260121 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/validation_error_loc.py
+-rw-r--r--   0        0        0     3408 2024-04-25 19:58:24.260208 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/validation_error_loc.pyi
+-rw-r--r--   0        0        0     4487 2024-04-25 20:02:27.023430 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/models/__init__.py
+-rw-r--r--   0        0        0    25772 2024-04-25 20:02:27.023562 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/operation_parameter_map.py
+-rw-r--r--   0        0        0      665 2024-04-25 20:02:27.024802 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/__init__.py
+-rw-r--r--   0        0        0      323 2024-04-25 19:58:24.260619 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_authors/__init__.py
+-rw-r--r--   0        0        0    66916 2024-04-25 19:58:24.260746 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_authors/get.py
+-rw-r--r--   0        0        0    66607 2024-04-25 19:58:24.260889 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_authors/get.pyi
+-rw-r--r--   0        0        0    47473 2024-04-25 19:58:24.261010 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_authors/post.py
+-rw-r--r--   0        0        0    47336 2024-04-25 19:58:24.261131 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_authors/post.pyi
+-rw-r--r--   0        0        0      341 2024-04-25 19:58:24.261232 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_latest_headlines/__init__.py
+-rw-r--r--   0        0        0    66032 2024-04-25 19:58:24.261357 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_latest_headlines/get.py
+-rw-r--r--   0        0        0    65723 2024-04-25 19:58:24.261497 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_latest_headlines/get.pyi
+-rw-r--r--   0        0        0    49192 2024-04-25 19:58:24.262028 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_latest_headlines/post.py
+-rw-r--r--   0        0        0    49055 2024-04-25 19:58:24.262159 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_latest_headlines/post.pyi
+-rw-r--r--   0        0        0      321 2024-04-25 19:58:24.262271 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search/__init__.py
+-rw-r--r--   0        0        0    78572 2024-04-25 20:02:27.029088 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search/get.py
+-rw-r--r--   0        0        0    78263 2024-04-25 20:02:27.029366 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search/get.pyi
+-rw-r--r--   0        0        0    55220 2024-04-25 20:02:27.031116 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search/post.py
+-rw-r--r--   0        0        0    55083 2024-04-25 20:02:27.031311 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search/post.pyi
+-rw-r--r--   0        0        0      337 2024-04-25 19:58:24.262979 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_by_link/__init__.py
+-rw-r--r--   0        0        0    19293 2024-04-25 19:58:24.263086 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_by_link/get.py
+-rw-r--r--   0        0        0    19070 2024-04-25 19:58:24.263219 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_by_link/get.pyi
+-rw-r--r--   0        0        0    17699 2024-04-25 19:58:24.263337 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_by_link/post.py
+-rw-r--r--   0        0        0    17562 2024-04-25 19:58:24.263462 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_by_link/post.pyi
+-rw-r--r--   0        0        0      373 2024-04-25 20:02:27.031417 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_duplicates_by_original_id/__init__.py
+-rw-r--r--   0        0        0    17623 2024-04-25 20:02:27.031489 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_duplicates_by_original_id/get.py
+-rw-r--r--   0        0        0    17400 2024-04-25 20:02:27.031596 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_duplicates_by_original_id/get.pyi
+-rw-r--r--   0        0        0    16697 2024-04-25 20:02:27.031674 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_duplicates_by_original_id/post.py
+-rw-r--r--   0        0        0    16560 2024-04-25 20:02:27.031764 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_duplicates_by_original_id/post.pyi
+-rw-r--r--   0        0        0      337 2024-04-25 19:58:24.264150 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_similar/__init__.py
+-rw-r--r--   0        0        0    67713 2024-04-25 19:58:24.264298 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_similar/get.py
+-rw-r--r--   0        0        0    67361 2024-04-25 19:58:24.264452 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_similar/get.pyi
+-rw-r--r--   0        0        0    47930 2024-04-25 19:58:24.264584 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_similar/post.py
+-rw-r--r--   0        0        0    47793 2024-04-25 19:58:24.264718 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_similar/post.pyi
+-rw-r--r--   0        0        0      323 2024-04-25 19:58:24.265433 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_sources/__init__.py
+-rw-r--r--   0        0        0    22889 2024-04-25 19:58:24.265541 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_sources/get.py
+-rw-r--r--   0        0        0    22752 2024-04-25 19:58:24.265659 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_sources/get.pyi
+-rw-r--r--   0        0        0    19936 2024-04-25 19:58:24.266109 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_sources/post.py
+-rw-r--r--   0        0        0    19799 2024-04-25 19:58:24.266226 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_sources/post.pyi
+-rw-r--r--   0        0        0      333 2024-04-25 19:58:24.266443 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_subscription/__init__.py
+-rw-r--r--   0        0        0    12067 2024-04-25 19:58:24.266541 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_subscription/get.py
+-rw-r--r--   0        0        0    11930 2024-04-25 19:58:24.266713 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_subscription/get.pyi
+-rw-r--r--   0        0        0    12093 2024-04-25 19:58:24.266880 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_subscription/post.py
+-rw-r--r--   0        0        0    11956 2024-04-25 19:58:24.267049 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_subscription/post.pyi
+-rw-r--r--   0        0        0        0 2024-04-25 19:58:24.267202 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/__init__.py
+-rw-r--r--   0        0        0      987 2024-04-25 19:58:24.267295 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/additional_source_info.py
+-rw-r--r--   0        0        0     4726 2024-04-25 19:58:24.267392 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/author_search_request.py
+-rw-r--r--   0        0        0     1061 2024-04-25 19:58:24.267483 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/authors_get_response.py
+-rw-r--r--   0        0        0     1062 2024-04-25 19:58:24.267572 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/authors_post_response.py
+-rw-r--r--   0        0        0      995 2024-04-25 19:58:24.267665 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/cluster.py
+-rw-r--r--   0        0        0      665 2024-04-25 19:58:24.267758 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/cluster_articles.py
+-rw-r--r--   0        0        0     1336 2024-04-25 19:58:24.267855 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/clustering_search_response.py
+-rw-r--r--   0        0        0     3052 2024-04-25 19:58:24.267949 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_author_search_response_article_result.py
+-rw-r--r--   0        0        0     1542 2024-04-25 19:58:24.268045 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_author_search_response_failed_search_response.py
+-rw-r--r--   0        0        0     1436 2024-04-25 19:58:24.268136 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response.py
+-rw-r--r--   0        0        0      704 2024-04-25 19:58:24.268234 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response_articles.py
+-rw-r--r--   0        0        0     3239 2024-04-25 19:58:24.268436 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_article_result.py
+-rw-r--r--   0        0        0     1543 2024-04-25 19:58:24.268716 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_failed_search_response.py
+-rw-r--r--   0        0        0     1437 2024-04-25 19:58:24.269513 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response.py
+-rw-r--r--   0        0        0      704 2024-04-25 19:58:24.269778 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response_articles.py
+-rw-r--r--   0        0        0     1411 2024-04-25 19:58:24.270012 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_search_response_search_response.py
+-rw-r--r--   0        0        0      698 2024-04-25 19:58:24.270224 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_search_response_search_response_articles.py
+-rw-r--r--   0        0        0      979 2024-04-25 20:02:27.031870 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/duplicates_by_original_id_request.py
+-rw-r--r--   0        0        0      937 2024-04-25 19:58:24.270419 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/http_validation_error.py
+-rw-r--r--   0        0        0      907 2024-04-25 19:58:24.270513 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/latest_headlines_get_response.py
+-rw-r--r--   0        0        0      908 2024-04-25 19:58:24.270720 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/latest_headlines_post_response.py
+-rw-r--r--   0        0        0     4897 2024-04-25 19:58:24.270824 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/latest_headlines_request.py
+-rw-r--r--   0        0        0     1340 2024-04-25 19:58:24.271021 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/latest_headlines_response.py
+-rw-r--r--   0        0        0      681 2024-04-25 19:58:24.271117 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/latest_headlines_response_articles.py
+-rw-r--r--   0        0        0     4721 2024-04-25 19:58:24.271214 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/more_like_this_request.py
+-rw-r--r--   0        0        0      952 2024-04-25 19:58:24.271301 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/search_get_response.py
+-rw-r--r--   0        0        0      953 2024-04-25 19:58:24.271491 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/search_post_response.py
+-rw-r--r--   0        0        0     5628 2024-04-25 20:02:27.032002 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/search_request.py
+-rw-r--r--   0        0        0     1069 2024-04-25 19:58:24.271790 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/search_similar_get_response.py
+-rw-r--r--   0        0        0     1070 2024-04-25 19:58:24.271903 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/search_similar_post_response.py
+-rw-r--r--   0        0        0     1151 2024-04-25 19:58:24.272107 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/search_url_request.py
+-rw-r--r--   0        0        0      974 2024-04-25 20:02:27.032073 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/searchduplicatesbyoriginalid_get_response.py
+-rw-r--r--   0        0        0      975 2024-04-25 20:02:27.032146 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/searchduplicatesbyoriginalid_post_response.py
+-rw-r--r--   0        0        0      937 2024-04-25 19:58:24.272469 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/similar_document.py
+-rw-r--r--   0        0        0     1132 2024-04-25 19:58:24.272670 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/source_info.py
+-rw-r--r--   0        0        0     1093 2024-04-25 19:58:24.272858 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/source_response.py
+-rw-r--r--   0        0        0      760 2024-04-25 19:58:24.273047 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/source_response_sources.py
+-rw-r--r--   0        0        0     1432 2024-04-25 19:58:24.273131 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/sources_request.py
+-rw-r--r--   0        0        0     1216 2024-04-25 19:58:24.273320 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/subscription_response.py
+-rw-r--r--   0        0        0      973 2024-04-25 19:58:24.273403 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/validation_error.py
+-rw-r--r--   0        0        0      684 2024-04-25 19:58:24.273600 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/validation_error_loc.py
+-rw-r--r--   0        0        0      913 2024-04-25 19:58:24.273689 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/request_after_hook.py
+-rw-r--r--   0        0        0      971 2024-04-25 19:58:24.273776 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/request_before_hook.py
+-rw-r--r--   0        0        0      936 2024-04-25 19:58:24.273966 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/request_before_url_hook.py
+-rw-r--r--   0        0        0    11233 2024-04-25 19:58:24.274049 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/rest.py
+-rw-r--r--   0        0        0    96391 2024-04-25 19:58:24.274266 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/schemas.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:58:24.274364 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/__init__.py
+-rw-r--r--   0        0        0      842 2024-04-25 19:58:24.274454 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/additional_source_info.py
+-rw-r--r--   0        0        0     2699 2024-04-25 19:58:24.274543 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/author_search_request.py
+-rw-r--r--   0        0        0      992 2024-04-25 19:58:24.274627 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/authors_get_response.py
+-rw-r--r--   0        0        0      993 2024-04-25 19:58:24.274715 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/authors_post_response.py
+-rw-r--r--   0        0        0      862 2024-04-25 19:58:24.274797 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/cluster.py
+-rw-r--r--   0        0        0      604 2024-04-25 19:58:24.274878 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/cluster_articles.py
+-rw-r--r--   0        0        0     1106 2024-04-25 19:58:24.274961 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/clustering_search_response.py
+-rw-r--r--   0        0        0     1778 2024-04-25 19:58:24.275053 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_author_search_response_article_result.py
+-rw-r--r--   0        0        0     1341 2024-04-25 19:58:24.275143 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_author_search_response_failed_search_response.py
+-rw-r--r--   0        0        0     1326 2024-04-25 19:58:24.275230 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_author_search_response_search_response.py
+-rw-r--r--   0        0        0      643 2024-04-25 19:58:24.275320 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_author_search_response_search_response_articles.py
+-rw-r--r--   0        0        0     1903 2024-04-25 19:58:24.275568 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_more_like_this_response_article_result.py
+-rw-r--r--   0        0        0     1342 2024-04-25 19:58:24.275659 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_more_like_this_response_failed_search_response.py
+-rw-r--r--   0        0        0     1327 2024-04-25 19:58:24.275745 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response.py
+-rw-r--r--   0        0        0      643 2024-04-25 19:58:24.275835 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response_articles.py
+-rw-r--r--   0        0        0     1277 2024-04-25 19:58:24.275922 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_search_response_search_response.py
+-rw-r--r--   0        0        0      637 2024-04-25 19:58:24.276011 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_search_response_search_response_articles.py
+-rw-r--r--   0        0        0      880 2024-04-25 20:02:27.032216 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/duplicates_by_original_id_request.py
+-rw-r--r--   0        0        0      889 2024-04-25 19:58:24.276181 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/http_validation_error.py
+-rw-r--r--   0        0        0      838 2024-04-25 19:58:24.276265 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/latest_headlines_get_response.py
+-rw-r--r--   0        0        0      839 2024-04-25 19:58:24.276350 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/latest_headlines_post_response.py
+-rw-r--r--   0        0        0     2812 2024-04-25 19:58:24.276431 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/latest_headlines_request.py
+-rw-r--r--   0        0        0     1138 2024-04-25 19:58:24.276517 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/latest_headlines_response.py
+-rw-r--r--   0        0        0      620 2024-04-25 19:58:24.276603 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/latest_headlines_response_articles.py
+-rw-r--r--   0        0        0     2616 2024-04-25 19:58:24.276691 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/more_like_this_request.py
+-rw-r--r--   0        0        0      883 2024-04-25 19:58:24.276776 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/search_get_response.py
+-rw-r--r--   0        0        0      884 2024-04-25 19:58:24.276970 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/search_post_response.py
+-rw-r--r--   0        0        0     3061 2024-04-25 20:02:27.032343 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/search_request.py
+-rw-r--r--   0        0        0     1000 2024-04-25 19:58:24.277144 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/search_similar_get_response.py
+-rw-r--r--   0        0        0     1001 2024-04-25 19:58:24.277224 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/search_similar_post_response.py
+-rw-r--r--   0        0        0      957 2024-04-25 19:58:24.277306 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/search_url_request.py
+-rw-r--r--   0        0        0      905 2024-04-25 20:02:27.032427 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/searchduplicatesbyoriginalid_get_response.py
+-rw-r--r--   0        0        0      906 2024-04-25 20:02:27.032497 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/searchduplicatesbyoriginalid_post_response.py
+-rw-r--r--   0        0        0      836 2024-04-25 19:58:24.277563 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/similar_document.py
+-rw-r--r--   0        0        0      904 2024-04-25 19:58:24.277644 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/source_info.py
+-rw-r--r--   0        0        0      994 2024-04-25 19:58:24.277730 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/source_response.py
+-rw-r--r--   0        0        0      695 2024-04-25 19:58:24.277816 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/source_response_sources.py
+-rw-r--r--   0        0        0      996 2024-04-25 19:58:24.277897 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/sources_request.py
+-rw-r--r--   0        0        0      925 2024-04-25 19:58:24.277987 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/subscription_response.py
+-rw-r--r--   0        0        0      892 2024-04-25 19:58:24.278071 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/validation_error.py
+-rw-r--r--   0        0        0      623 2024-04-25 19:58:24.278162 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/validation_error_loc.py
+-rw-r--r--   0        0        0      758 2024-04-25 19:58:24.278243 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type_util.py
+-rw-r--r--   0        0        0     3177 2024-04-25 19:58:24.278323 newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/validation_metadata.py
+-rw-r--r--   0        0        0      791 2024-04-25 20:02:27.032728 newscatcherapi_python_sdk-6.0.5/pyproject.toml
+-rw-r--r--   0        0        0    78988 1970-01-01 00:00:00.000000 newscatcherapi_python_sdk-6.0.5/PKG-INFO
```

### Comparing `newscatcherapi_python_sdk-6.0.4/LICENSE` & `newscatcherapi_python_sdk-6.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/README.md` & `newscatcherapi_python_sdk-6.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,39 @@
+Metadata-Version: 2.1
+Name: newscatcherapi-python-sdk
+Version: 6.0.5
+Summary: Client for NewsCatcher-V3 Production API
+License: MIT
+Author: Maksym Sugonyaka
+Author-email: maksym@newscatcherapi.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: certifi (>=2023.7.22)
+Requires-Dist: cryptography (>=42.0.5,<43.0.0)
+Requires-Dist: frozendict (>=2.3.4,<3.0.0)
+Requires-Dist: pydantic (>=2.4.2,<3.0.0)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: typing_extensions (>=4.3.0,<5.0.0)
+Requires-Dist: urllib3 (>=1.26.18,<2.0.0)
+Description-Content-Type: text/markdown
+
 # newscatcherapi-python-sdk<a id="newscatcherapi-python-sdk"></a>
 
 <img src='https://uploads-ssl.webflow.com/6429857b17973b636c2195c5/646c6f1eb774ff2f2997bec5_newscatcher_.svg' width='286' height='35' /> <br>  <br>Visit our website  <a href='https://newscatcherapi.com'>https://newscatcherapi.com</a>
 
 
-[![PyPI](https://img.shields.io/badge/PyPI-v6.0.4-blue)](https://pypi.org/project/newscatcherapi-python-sdk/6.0.4)
+[![PyPI](https://img.shields.io/badge/PyPI-v6.0.5-blue)](https://pypi.org/project/newscatcherapi-python-sdk/6.0.5)
 [![README.md](https://img.shields.io/badge/README-Click%20Here-green)](https://github.com/konfig-dev/newscatcher-sdks/tree/main/v3/python#readme)
 
 ## Table of Contents<a id="table-of-contents"></a>
 
 <!-- toc -->
 
 - [Requirements](#requirements)
@@ -26,25 +52,27 @@
   * [`newscatcher.search_link.post`](#newscatchersearch_linkpost)
   * [`newscatcher.search_similar.get`](#newscatchersearch_similarget)
   * [`newscatcher.search_similar.post`](#newscatchersearch_similarpost)
   * [`newscatcher.sources.get`](#newscatchersourcesget)
   * [`newscatcher.sources.post`](#newscatchersourcespost)
   * [`newscatcher.subscription.get`](#newscatchersubscriptionget)
   * [`newscatcher.subscription.post`](#newscatchersubscriptionpost)
+  * [`newscatcher.search_duplicates_by_original_id.get`](#newscatchersearch_duplicates_by_original_idget)
+  * [`newscatcher.search_duplicates_by_original_id.post`](#newscatchersearch_duplicates_by_original_idpost)
 
 <!-- tocstop -->
 
 ## Requirements<a id="requirements"></a>
 
 Python >=3.7
 
 ## Installation<a id="installation"></a>
 
 ```sh
-pip install newscatcherapi-python-sdk==6.0.4
+pip install newscatcherapi-python-sdk==6.0.5
 ```
 
 ## Getting Started<a id="getting-started"></a>
 
 ```python
 from pprint import pprint
 from newscatcherapi_client import Newscatcher, ApiException
@@ -882,14 +910,15 @@
     content_sentiment_min=3.14,
     content_sentiment_max=3.14,
     iptc_tags=None,
     not_iptc_tags=None,
     source_name=None,
     iab_tags=None,
     not_iab_tags=None,
+    exclude_duplicates=True,
 )
 ```
 
 #### ⚙️ Parameters<a id="⚙️-parameters"></a>
 
 ##### q: `str`<a id="q-str"></a>
 
@@ -983,14 +1012,16 @@
 
 ##### source_name: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="source_name-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
 
 ##### iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
 
 ##### not_iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="not_iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
 
+##### exclude_duplicates: `bool`<a id="exclude_duplicates-bool"></a>
+
 #### 🔄 Return<a id="🔄-return"></a>
 
 [`SearchGetResponse`](./newscatcherapi_client/pydantic/search_get_response.py)
 
 #### 🌐 Endpoint<a id="🌐-endpoint"></a>
 
 `/api/search` `get`
@@ -1050,14 +1081,15 @@
     content_sentiment_min=3.14,
     content_sentiment_max=3.14,
     iptc_tags=None,
     not_iptc_tags=None,
     source_name=None,
     iab_tags=None,
     not_iab_tags=None,
+    exclude_duplicates=True,
 )
 ```
 
 #### ⚙️ Parameters<a id="⚙️-parameters"></a>
 
 ##### q: `str`<a id="q-str"></a>
 
@@ -1151,14 +1183,16 @@
 
 ##### source_name: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="source_name-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
 
 ##### iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
 
 ##### not_iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="not_iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
 
+##### exclude_duplicates: `bool`<a id="exclude_duplicates-bool"></a>
+
 #### ⚙️ Request Body<a id="⚙️-request-body"></a>
 
 [`SearchRequest`](./newscatcherapi_client/type/search_request.py)
 #### 🔄 Return<a id="🔄-return"></a>
 
 [`SearchPostResponse`](./newscatcherapi_client/pydantic/search_post_response.py)
 
@@ -1685,10 +1719,82 @@
 
 `/api/subscription` `post`
 
 [🔙 **Back to Table of Contents**](#table-of-contents)
 
 ---
 
+### `newscatcher.search_duplicates_by_original_id.get`<a id="newscatchersearch_duplicates_by_original_idget"></a>
+
+This endpoint allows you to search for duplicate articles by original article id.
+
+#### 🛠️ Usage<a id="🛠️-usage"></a>
+
+```python
+get_response = newscatcher.search_duplicates_by_original_id.get(
+    original_article_id="original_article_id_example",
+    page=1,
+    page_size=100,
+)
+```
+
+#### ⚙️ Parameters<a id="⚙️-parameters"></a>
+
+##### original_article_id: `str`<a id="original_article_id-str"></a>
+
+##### page: `int`<a id="page-int"></a>
+
+##### page_size: `int`<a id="page_size-int"></a>
+
+#### 🔄 Return<a id="🔄-return"></a>
+
+[`SearchduplicatesbyoriginalidGetResponse`](./newscatcherapi_client/pydantic/searchduplicatesbyoriginalid_get_response.py)
+
+#### 🌐 Endpoint<a id="🌐-endpoint"></a>
+
+`/api/search_duplicates_by_original_id` `get`
+
+[🔙 **Back to Table of Contents**](#table-of-contents)
+
+---
+
+### `newscatcher.search_duplicates_by_original_id.post`<a id="newscatchersearch_duplicates_by_original_idpost"></a>
+
+This endpoint allows you to search for duplicate articles by original article id.
+
+#### 🛠️ Usage<a id="🛠️-usage"></a>
+
+```python
+post_response = newscatcher.search_duplicates_by_original_id.post(
+    original_article_id="string_example",
+    page=1,
+    page_size=100,
+)
+```
+
+#### ⚙️ Parameters<a id="⚙️-parameters"></a>
+
+##### original_article_id: `str`<a id="original_article_id-str"></a>
+
+##### page: `int`<a id="page-int"></a>
+
+##### page_size: `int`<a id="page_size-int"></a>
+
+#### ⚙️ Request Body<a id="⚙️-request-body"></a>
+
+[`DuplicatesByOriginalIdRequest`](./newscatcherapi_client/type/duplicates_by_original_id_request.py)
+#### 🔄 Return<a id="🔄-return"></a>
+
+[`SearchduplicatesbyoriginalidPostResponse`](./newscatcherapi_client/pydantic/searchduplicatesbyoriginalid_post_response.py)
+
+#### 🌐 Endpoint<a id="🌐-endpoint"></a>
+
+`/api/search_duplicates_by_original_id` `post`
+
+[🔙 **Back to Table of Contents**](#table-of-contents)
+
+---
+
 
 ## Author<a id="author"></a>
 This Python package is automatically generated by [Konfig](https://konfigthis.com)
+
```

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/__init__.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     <img src='https://uploads-ssl.webflow.com/6429857b17973b636c2195c5/646c6f1eb774ff2f2997bec5_newscatcher_.svg' width='286' height='35' /> <br>  <br>Visit our website  <a href='https://newscatcherapi.com'>https://newscatcherapi.com</a>
 
     The version of the OpenAPI document: 3.2.16
     Contact: maksym@newscatcherapi.com
     Generated by: https://konfigthis.com
 """
 
-__version__ = "6.0.4"
+__version__ = "6.0.5"
 
 # import ApiClient
 from newscatcherapi_client.api_client import ApiClient
 
 # import Configuration
 from newscatcherapi_client.configuration import Configuration
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8 # flake8: noqa """ NewsCatcher-V3 Production API [https://
 uploads-ssl.webflow.com/6429857b17973b636c2195c5/
 646c6f1eb774ff2f2997bec5_newscatcher_.svg]
 
 Visit our website _h_t_t_p_s_:_/_/_n_e_w_s_c_a_t_c_h_e_r_a_p_i_._c_o_m The version of the OpenAPI
 document: 3.2.16 Contact: maksym@newscatcherapi.com Generated by: https://
-konfigthis.com """ __version__ = "6.0.4" # import ApiClient from
+konfigthis.com """ __version__ = "6.0.5" # import ApiClient from
 newscatcherapi_client.api_client import ApiClient # import Configuration from
 newscatcherapi_client.configuration import Configuration # import exceptions
 from newscatcherapi_client.exceptions import OpenApiException from
 newscatcherapi_client.exceptions import ApiAttributeError from
 newscatcherapi_client.exceptions import ApiTypeError from
 newscatcherapi_client.exceptions import ApiValueError from
 newscatcherapi_client.exceptions import ApiKeyError from
```

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/api_client.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2984,15 +2984,15 @@
 0000ba70: 655d 203d 2068 6561 6465 725f 7661 6c75  e] = header_valu
 0000ba80: 650a 2020 2020 2020 2020 7365 6c66 2e63  e.        self.c
 0000ba90: 6f6f 6b69 6520 3d20 636f 6f6b 6965 0a20  ookie = cookie. 
 0000baa0: 2020 2020 2020 2023 2053 6574 2064 6566         # Set def
 0000bab0: 6175 6c74 2055 7365 722d 4167 656e 742e  ault User-Agent.
 0000bac0: 0a20 2020 2020 2020 2073 656c 662e 7573  .        self.us
 0000bad0: 6572 5f61 6765 6e74 203d 2027 4b6f 6e66  er_agent = 'Konf
-0000bae0: 6967 2f36 2e30 2e34 2f70 7974 686f 6e27  ig/6.0.4/python'
+0000bae0: 6967 2f36 2e30 2e35 2f70 7974 686f 6e27  ig/6.0.5/python'
 0000baf0: 0a0a 2020 2020 6465 6620 5f5f 656e 7465  ..    def __ente
 0000bb00: 725f 5f28 7365 6c66 293a 0a20 2020 2020  r__(self):.     
 0000bb10: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
 0000bb20: 2020 2020 6465 6620 5f5f 6578 6974 5f5f      def __exit__
 0000bb30: 2873 656c 662c 2065 7863 5f74 7970 652c  (self, exc_type,
 0000bb40: 2065 7863 5f76 616c 7565 2c20 7472 6163   exc_value, trac
 0000bb50: 6562 6163 6b29 3a0a 2020 2020 2020 2020  eback):.
```

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/api_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/api_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/path_to_api.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/path_to_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,32 +4,35 @@
 from newscatcherapi_client.apis.paths.api_search import ApiSearch
 from newscatcherapi_client.apis.paths.api_latest_headlines import ApiLatestHeadlines
 from newscatcherapi_client.apis.paths.api_authors import ApiAuthors
 from newscatcherapi_client.apis.paths.api_search_by_link import ApiSearchByLink
 from newscatcherapi_client.apis.paths.api_search_similar import ApiSearchSimilar
 from newscatcherapi_client.apis.paths.api_sources import ApiSources
 from newscatcherapi_client.apis.paths.api_subscription import ApiSubscription
+from newscatcherapi_client.apis.paths.api_search_duplicates_by_original_id import ApiSearchDuplicatesByOriginalId
 
 PathToApi = typing_extensions.TypedDict(
     'PathToApi',
     {
         PathValues.API_SEARCH: ApiSearch,
         PathValues.API_LATEST_HEADLINES: ApiLatestHeadlines,
         PathValues.API_AUTHORS: ApiAuthors,
         PathValues.API_SEARCH_BY_LINK: ApiSearchByLink,
         PathValues.API_SEARCH_SIMILAR: ApiSearchSimilar,
         PathValues.API_SOURCES: ApiSources,
         PathValues.API_SUBSCRIPTION: ApiSubscription,
+        PathValues.API_SEARCH_DUPLICATES_BY_ORIGINAL_ID: ApiSearchDuplicatesByOriginalId,
     }
 )
 
 path_to_api = PathToApi(
     {
         PathValues.API_SEARCH: ApiSearch,
         PathValues.API_LATEST_HEADLINES: ApiLatestHeadlines,
         PathValues.API_AUTHORS: ApiAuthors,
         PathValues.API_SEARCH_BY_LINK: ApiSearchByLink,
         PathValues.API_SEARCH_SIMILAR: ApiSearchSimilar,
         PathValues.API_SOURCES: ApiSources,
         PathValues.API_SUBSCRIPTION: ApiSubscription,
+        PathValues.API_SEARCH_DUPLICATES_BY_ORIGINAL_ID: ApiSearchDuplicatesByOriginalId,
     }
 )
```

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tag_to_api.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tag_to_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,32 +4,35 @@
 from newscatcherapi_client.apis.tags.search_api import SearchApi
 from newscatcherapi_client.apis.tags.latest_headlines_api import LatestHeadlinesApi
 from newscatcherapi_client.apis.tags.authors_api import AuthorsApi
 from newscatcherapi_client.apis.tags.search_link_api import SearchLinkApi
 from newscatcherapi_client.apis.tags.search_similar_api import SearchSimilarApi
 from newscatcherapi_client.apis.tags.sources_api import SourcesApi
 from newscatcherapi_client.apis.tags.subscription_api import SubscriptionApi
+from newscatcherapi_client.apis.tags.search_duplicates_by_original_id_api import SearchDuplicatesByOriginalIdApi
 
 TagToApi = typing_extensions.TypedDict(
     'TagToApi',
     {
         TagValues.SEARCH: SearchApi,
         TagValues.LATEST_HEADLINES: LatestHeadlinesApi,
         TagValues.AUTHORS: AuthorsApi,
         TagValues.SEARCH_LINK: SearchLinkApi,
         TagValues.SEARCH_SIMILAR: SearchSimilarApi,
         TagValues.SOURCES: SourcesApi,
         TagValues.SUBSCRIPTION: SubscriptionApi,
+        TagValues.SEARCH_DUPLICATES_BY_ORIGINAL_ID: SearchDuplicatesByOriginalIdApi,
     }
 )
 
 tag_to_api = TagToApi(
     {
         TagValues.SEARCH: SearchApi,
         TagValues.LATEST_HEADLINES: LatestHeadlinesApi,
         TagValues.AUTHORS: AuthorsApi,
         TagValues.SEARCH_LINK: SearchLinkApi,
         TagValues.SEARCH_SIMILAR: SearchSimilarApi,
         TagValues.SOURCES: SourcesApi,
         TagValues.SUBSCRIPTION: SubscriptionApi,
+        TagValues.SEARCH_DUPLICATES_BY_ORIGINAL_ID: SearchDuplicatesByOriginalIdApi,
     }
 )
```

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/authors_api.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/authors_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/authors_api_raw.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/authors_api_raw.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/latest_headlines_api.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/latest_headlines_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/latest_headlines_api_raw.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/latest_headlines_api_raw.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/search_api.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/search_api_raw.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_api_raw.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/search_link_api.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_link_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/search_link_api_raw.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_link_api_raw.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/search_similar_api.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_similar_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/search_similar_api_raw.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/search_similar_api_raw.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/sources_api.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/sources_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/sources_api_raw.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/sources_api_raw.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/subscription_api.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/subscription_api.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/apis/tags/subscription_api_raw.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/apis/tags/subscription_api_raw.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/client.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from newscatcherapi_client.apis.tags.authors_api import AuthorsApi
 from newscatcherapi_client.apis.tags.latest_headlines_api import LatestHeadlinesApi
 from newscatcherapi_client.apis.tags.search_api import SearchApi
 from newscatcherapi_client.apis.tags.search_link_api import SearchLinkApi
 from newscatcherapi_client.apis.tags.search_similar_api import SearchSimilarApi
 from newscatcherapi_client.apis.tags.sources_api import SourcesApi
 from newscatcherapi_client.apis.tags.subscription_api import SubscriptionApi
+from newscatcherapi_client.apis.tags.search_duplicates_by_original_id_api import SearchDuplicatesByOriginalIdApi
 
 
 
 class Newscatcher(ClientCustom):
 
     def __init__(self, configuration: typing.Union[Configuration, None] = None, **kwargs):
         super().__init__(configuration, **kwargs)
@@ -38,7 +39,8 @@
         self.authors: AuthorsApi = AuthorsApi(api_client)
         self.latest_headlines: LatestHeadlinesApi = LatestHeadlinesApi(api_client)
         self.search: SearchApi = SearchApi(api_client)
         self.search_link: SearchLinkApi = SearchLinkApi(api_client)
         self.search_similar: SearchSimilarApi = SearchSimilarApi(api_client)
         self.sources: SourcesApi = SourcesApi(api_client)
         self.subscription: SubscriptionApi = SubscriptionApi(api_client)
+        self.search_duplicates_by_original_id: SearchDuplicatesByOriginalIdApi = SearchDuplicatesByOriginalIdApi(api_client)
```

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/client.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/client.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from newscatcherapi_client.apis.tags.authors_api import AuthorsApi
 from newscatcherapi_client.apis.tags.latest_headlines_api import LatestHeadlinesApi
 from newscatcherapi_client.apis.tags.search_api import SearchApi
 from newscatcherapi_client.apis.tags.search_link_api import SearchLinkApi
 from newscatcherapi_client.apis.tags.search_similar_api import SearchSimilarApi
 from newscatcherapi_client.apis.tags.sources_api import SourcesApi
 from newscatcherapi_client.apis.tags.subscription_api import SubscriptionApi
+from newscatcherapi_client.apis.tags.search_duplicates_by_original_id_api import SearchDuplicatesByOriginalIdApi
 
 
 
 class Newscatcher(ClientCustom):
 
     def __init__(self, configuration: typing.Union[Configuration, None] = None, **kwargs):
         super().__init__(configuration, **kwargs)
@@ -38,7 +39,8 @@
         self.authors: AuthorsApi = AuthorsApi(api_client)
         self.latest_headlines: LatestHeadlinesApi = LatestHeadlinesApi(api_client)
         self.search: SearchApi = SearchApi(api_client)
         self.search_link: SearchLinkApi = SearchLinkApi(api_client)
         self.search_similar: SearchSimilarApi = SearchSimilarApi(api_client)
         self.sources: SourcesApi = SourcesApi(api_client)
         self.subscription: SubscriptionApi = SubscriptionApi(api_client)
+        self.search_duplicates_by_original_id: SearchDuplicatesByOriginalIdApi = SearchDuplicatesByOriginalIdApi(api_client)
```

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/client_custom.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/client_custom.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/configuration.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,15 +404,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 3.2.16\n"\
-               "SDK Package Version: 6.0.4".\
+               "SDK Package Version: 6.0.5".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/exceptions.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/exceptions_base.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/exceptions_base.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/additional_source_info.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/additional_source_info.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/additional_source_info.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/additional_source_info.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/author_search_request.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/author_search_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/author_search_request.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/author_search_request.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/authors_get_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/authors_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/authors_get_response.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/authors_get_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/authors_post_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/authors_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/authors_post_response.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/authors_post_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/cluster.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/cluster.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/cluster.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/cluster.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/cluster_articles.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/cluster_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/cluster_articles.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/cluster_articles.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/clustering_search_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/clustering_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/clustering_search_response.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/clustering_search_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_article_result.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_article_result.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_article_result.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_article_result.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_failed_search_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_search_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_search_response.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_search_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_author_search_response_search_response_articles.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_article_result.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_failed_search_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_more_like_this_response_search_response_articles.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_search_response_search_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_search_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_search_response_search_response.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_search_response_search_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/dto_responses_search_response_search_response_articles.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/http_validation_error.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/http_validation_error.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/http_validation_error.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_get_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_get_response.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_get_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_post_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_post_response.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_post_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_request.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_request.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_request.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_response.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_response_articles.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/latest_headlines_response_articles.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/latest_headlines_response_articles.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/more_like_this_request.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/more_like_this_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/more_like_this_request.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/more_like_this_request.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_get_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_get_response.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_get_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_post_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_post_response.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_post_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_request.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,14 +191,15 @@
             content_sentiment_min = schemas.NumberSchema
             content_sentiment_max = schemas.NumberSchema
             iptc_tags = schemas.AnyTypeSchema
             not_iptc_tags = schemas.AnyTypeSchema
             source_name = schemas.AnyTypeSchema
             iab_tags = schemas.AnyTypeSchema
             not_iab_tags = schemas.AnyTypeSchema
+            exclude_duplicates = schemas.BoolSchema
             __annotations__ = {
                 "q": q,
                 "search_in": search_in,
                 "predefined_sources": predefined_sources,
                 "sources": sources,
                 "not_sources": not_sources,
                 "lang": lang,
@@ -239,14 +240,15 @@
                 "content_sentiment_min": content_sentiment_min,
                 "content_sentiment_max": content_sentiment_max,
                 "iptc_tags": iptc_tags,
                 "not_iptc_tags": not_iptc_tags,
                 "source_name": source_name,
                 "iab_tags": iab_tags,
                 "not_iab_tags": not_iab_tags,
+                "exclude_duplicates": exclude_duplicates,
             }
     
     q: MetaOapg.properties.q
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["q"]) -> MetaOapg.properties.q: ...
     
@@ -385,17 +387,20 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["iab_tags"]) -> MetaOapg.properties.iab_tags: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["not_iab_tags"]) -> MetaOapg.properties.not_iab_tags: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["exclude_duplicates"]) -> MetaOapg.properties.exclude_duplicates: ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["q", "search_in", "predefined_sources", "sources", "not_sources", "lang", "not_lang", "countries", "not_countries", "not_author_name", "from_", "to_", "published_date_precision", "by_parse_date", "sort_by", "ranked_only", "from_rank", "to_rank", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "clustering_variable", "clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name", "MISC_entity_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", "source_name", "iab_tags", "not_iab_tags", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["q", "search_in", "predefined_sources", "sources", "not_sources", "lang", "not_lang", "countries", "not_countries", "not_author_name", "from_", "to_", "published_date_precision", "by_parse_date", "sort_by", "ranked_only", "from_rank", "to_rank", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "clustering_variable", "clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name", "MISC_entity_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", "source_name", "iab_tags", "not_iab_tags", "exclude_duplicates", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["q"]) -> MetaOapg.properties.q: ...
     
@@ -534,17 +539,20 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["iab_tags"]) -> typing.Union[MetaOapg.properties.iab_tags, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["not_iab_tags"]) -> typing.Union[MetaOapg.properties.not_iab_tags, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["exclude_duplicates"]) -> typing.Union[MetaOapg.properties.exclude_duplicates, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["q", "search_in", "predefined_sources", "sources", "not_sources", "lang", "not_lang", "countries", "not_countries", "not_author_name", "from_", "to_", "published_date_precision", "by_parse_date", "sort_by", "ranked_only", "from_rank", "to_rank", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "clustering_variable", "clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name", "MISC_entity_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", "source_name", "iab_tags", "not_iab_tags", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["q", "search_in", "predefined_sources", "sources", "not_sources", "lang", "not_lang", "countries", "not_countries", "not_author_name", "from_", "to_", "published_date_precision", "by_parse_date", "sort_by", "ranked_only", "from_rank", "to_rank", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "clustering_variable", "clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name", "MISC_entity_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", "source_name", "iab_tags", "not_iab_tags", "exclude_duplicates", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         q: typing.Union[MetaOapg.properties.q, str, ],
@@ -590,14 +598,15 @@
         content_sentiment_min: typing.Union[MetaOapg.properties.content_sentiment_min, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         content_sentiment_max: typing.Union[MetaOapg.properties.content_sentiment_max, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         iptc_tags: typing.Union[MetaOapg.properties.iptc_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         not_iptc_tags: typing.Union[MetaOapg.properties.not_iptc_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         source_name: typing.Union[MetaOapg.properties.source_name, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         iab_tags: typing.Union[MetaOapg.properties.iab_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         not_iab_tags: typing.Union[MetaOapg.properties.not_iab_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        exclude_duplicates: typing.Union[MetaOapg.properties.exclude_duplicates, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'SearchRequest':
         return super().__new__(
             cls,
             *args,
             q=q,
@@ -643,10 +652,11 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
             not_iab_tags=not_iab_tags,
+            exclude_duplicates=exclude_duplicates,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_request.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_request.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -179,14 +179,15 @@
             content_sentiment_min = schemas.NumberSchema
             content_sentiment_max = schemas.NumberSchema
             iptc_tags = schemas.AnyTypeSchema
             not_iptc_tags = schemas.AnyTypeSchema
             source_name = schemas.AnyTypeSchema
             iab_tags = schemas.AnyTypeSchema
             not_iab_tags = schemas.AnyTypeSchema
+            exclude_duplicates = schemas.BoolSchema
             __annotations__ = {
                 "q": q,
                 "search_in": search_in,
                 "predefined_sources": predefined_sources,
                 "sources": sources,
                 "not_sources": not_sources,
                 "lang": lang,
@@ -227,14 +228,15 @@
                 "content_sentiment_min": content_sentiment_min,
                 "content_sentiment_max": content_sentiment_max,
                 "iptc_tags": iptc_tags,
                 "not_iptc_tags": not_iptc_tags,
                 "source_name": source_name,
                 "iab_tags": iab_tags,
                 "not_iab_tags": not_iab_tags,
+                "exclude_duplicates": exclude_duplicates,
             }
     
     q: MetaOapg.properties.q
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["q"]) -> MetaOapg.properties.q: ...
     
@@ -373,17 +375,20 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["iab_tags"]) -> MetaOapg.properties.iab_tags: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["not_iab_tags"]) -> MetaOapg.properties.not_iab_tags: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["exclude_duplicates"]) -> MetaOapg.properties.exclude_duplicates: ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["q", "search_in", "predefined_sources", "sources", "not_sources", "lang", "not_lang", "countries", "not_countries", "not_author_name", "from_", "to_", "published_date_precision", "by_parse_date", "sort_by", "ranked_only", "from_rank", "to_rank", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "clustering_variable", "clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name", "MISC_entity_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", "source_name", "iab_tags", "not_iab_tags", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["q", "search_in", "predefined_sources", "sources", "not_sources", "lang", "not_lang", "countries", "not_countries", "not_author_name", "from_", "to_", "published_date_precision", "by_parse_date", "sort_by", "ranked_only", "from_rank", "to_rank", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "clustering_variable", "clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name", "MISC_entity_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", "source_name", "iab_tags", "not_iab_tags", "exclude_duplicates", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["q"]) -> MetaOapg.properties.q: ...
     
@@ -522,17 +527,20 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["iab_tags"]) -> typing.Union[MetaOapg.properties.iab_tags, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["not_iab_tags"]) -> typing.Union[MetaOapg.properties.not_iab_tags, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["exclude_duplicates"]) -> typing.Union[MetaOapg.properties.exclude_duplicates, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["q", "search_in", "predefined_sources", "sources", "not_sources", "lang", "not_lang", "countries", "not_countries", "not_author_name", "from_", "to_", "published_date_precision", "by_parse_date", "sort_by", "ranked_only", "from_rank", "to_rank", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "clustering_variable", "clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name", "MISC_entity_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", "source_name", "iab_tags", "not_iab_tags", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["q", "search_in", "predefined_sources", "sources", "not_sources", "lang", "not_lang", "countries", "not_countries", "not_author_name", "from_", "to_", "published_date_precision", "by_parse_date", "sort_by", "ranked_only", "from_rank", "to_rank", "is_headline", "is_paid_content", "parent_url", "all_links", "all_domain_links", "word_count_min", "word_count_max", "page", "page_size", "clustering_variable", "clustering_enabled", "clustering_threshold", "include_nlp_data", "has_nlp", "theme", "not_theme", "ORG_entity_name", "PER_entity_name", "LOC_entity_name", "MISC_entity_name", "title_sentiment_min", "title_sentiment_max", "content_sentiment_min", "content_sentiment_max", "iptc_tags", "not_iptc_tags", "source_name", "iab_tags", "not_iab_tags", "exclude_duplicates", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         q: typing.Union[MetaOapg.properties.q, str, ],
@@ -578,14 +586,15 @@
         content_sentiment_min: typing.Union[MetaOapg.properties.content_sentiment_min, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         content_sentiment_max: typing.Union[MetaOapg.properties.content_sentiment_max, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         iptc_tags: typing.Union[MetaOapg.properties.iptc_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         not_iptc_tags: typing.Union[MetaOapg.properties.not_iptc_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         source_name: typing.Union[MetaOapg.properties.source_name, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         iab_tags: typing.Union[MetaOapg.properties.iab_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         not_iab_tags: typing.Union[MetaOapg.properties.not_iab_tags, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        exclude_duplicates: typing.Union[MetaOapg.properties.exclude_duplicates, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'SearchRequest':
         return super().__new__(
             cls,
             *args,
             q=q,
@@ -631,10 +640,11 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
             not_iab_tags=not_iab_tags,
+            exclude_duplicates=exclude_duplicates,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_similar_get_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_similar_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_similar_get_response.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_similar_get_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_similar_post_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_similar_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_similar_post_response.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_similar_post_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_url_request.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_url_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/search_url_request.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/search_url_request.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/similar_document.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/similar_document.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/similar_document.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/similar_document.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/source_info.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/source_info.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/source_info.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/source_info.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/source_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/source_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/source_response.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/source_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/source_response_sources.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/source_response_sources.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/source_response_sources.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/source_response_sources.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/sources_request.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/sources_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/sources_request.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/sources_request.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/subscription_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/subscription_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/subscription_response.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/subscription_response.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/validation_error.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/validation_error.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/validation_error.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/validation_error_loc.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/validation_error_loc.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/model/validation_error_loc.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/model/validation_error_loc.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/models/__init__.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,27 +24,30 @@
 from newscatcherapi_client.model.dto_responses_author_search_response_search_response_articles import DtoResponsesAuthorSearchResponseSearchResponseArticles
 from newscatcherapi_client.model.dto_responses_more_like_this_response_article_result import DtoResponsesMoreLikeThisResponseArticleResult
 from newscatcherapi_client.model.dto_responses_more_like_this_response_failed_search_response import DtoResponsesMoreLikeThisResponseFailedSearchResponse
 from newscatcherapi_client.model.dto_responses_more_like_this_response_search_response import DtoResponsesMoreLikeThisResponseSearchResponse
 from newscatcherapi_client.model.dto_responses_more_like_this_response_search_response_articles import DtoResponsesMoreLikeThisResponseSearchResponseArticles
 from newscatcherapi_client.model.dto_responses_search_response_search_response import DtoResponsesSearchResponseSearchResponse
 from newscatcherapi_client.model.dto_responses_search_response_search_response_articles import DtoResponsesSearchResponseSearchResponseArticles
+from newscatcherapi_client.model.duplicates_by_original_id_request import DuplicatesByOriginalIdRequest
 from newscatcherapi_client.model.http_validation_error import HTTPValidationError
 from newscatcherapi_client.model.latest_headlines_get_response import LatestHeadlinesGetResponse
 from newscatcherapi_client.model.latest_headlines_post_response import LatestHeadlinesPostResponse
 from newscatcherapi_client.model.latest_headlines_request import LatestHeadlinesRequest
 from newscatcherapi_client.model.latest_headlines_response import LatestHeadlinesResponse
 from newscatcherapi_client.model.latest_headlines_response_articles import LatestHeadlinesResponseArticles
 from newscatcherapi_client.model.more_like_this_request import MoreLikeThisRequest
 from newscatcherapi_client.model.search_get_response import SearchGetResponse
 from newscatcherapi_client.model.search_post_response import SearchPostResponse
 from newscatcherapi_client.model.search_request import SearchRequest
 from newscatcherapi_client.model.search_similar_get_response import SearchSimilarGetResponse
 from newscatcherapi_client.model.search_similar_post_response import SearchSimilarPostResponse
 from newscatcherapi_client.model.search_url_request import SearchURLRequest
+from newscatcherapi_client.model.searchduplicatesbyoriginalid_get_response import SearchduplicatesbyoriginalidGetResponse
+from newscatcherapi_client.model.searchduplicatesbyoriginalid_post_response import SearchduplicatesbyoriginalidPostResponse
 from newscatcherapi_client.model.similar_document import SimilarDocument
 from newscatcherapi_client.model.source_info import SourceInfo
 from newscatcherapi_client.model.source_response import SourceResponse
 from newscatcherapi_client.model.source_response_sources import SourceResponseSources
 from newscatcherapi_client.model.sources_request import SourcesRequest
 from newscatcherapi_client.model.subscription_response import SubscriptionResponse
 from newscatcherapi_client.model.validation_error import ValidationError
```

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/operation_parameter_map.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/operation_parameter_map.py`

 * *Files 3% similar despite different names*

```diff
@@ -622,14 +622,17 @@
             },
             {
                 'name': 'iab_tags'
             },
             {
                 'name': 'not_iab_tags'
             },
+            {
+                'name': 'exclude_duplicates'
+            },
         ]
     },
     '/api/search-POST': {
         'parameters': [
             {
                 'name': 'q'
             },
@@ -767,14 +770,17 @@
             },
             {
                 'name': 'iab_tags'
             },
             {
                 'name': 'not_iab_tags'
             },
+            {
+                'name': 'exclude_duplicates'
+            },
         ]
     },
     '/api/search_by_link-GET': {
         'parameters': [
             {
                 'name': 'ids'
             },
@@ -1113,8 +1119,34 @@
         'parameters': [
         ]
     },
     '/api/subscription-POST': {
         'parameters': [
         ]
     },
+    '/api/search_duplicates_by_original_id-GET': {
+        'parameters': [
+            {
+                'name': 'original_article_id'
+            },
+            {
+                'name': 'page'
+            },
+            {
+                'name': 'page_size'
+            },
+        ]
+    },
+    '/api/search_duplicates_by_original_id-POST': {
+        'parameters': [
+            {
+                'name': 'original_article_id'
+            },
+            {
+                'name': 'page'
+            },
+            {
+                'name': 'page_size'
+            },
+        ]
+    },
 };
```

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/__init__.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,7 +9,8 @@
     API_SEARCH = "/api/search"
     API_LATEST_HEADLINES = "/api/latest_headlines"
     API_AUTHORS = "/api/authors"
     API_SEARCH_BY_LINK = "/api/search_by_link"
     API_SEARCH_SIMILAR = "/api/search_similar"
     API_SOURCES = "/api/sources"
     API_SUBSCRIPTION = "/api/subscription"
+    API_SEARCH_DUPLICATES_BY_ORIGINAL_ID = "/api/search_duplicates_by_original_id"
```

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_authors/get.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_authors/get.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_authors/get.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_authors/get.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_authors/post.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_authors/post.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_authors/post.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_authors/post.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_latest_headlines/get.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_latest_headlines/get.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_latest_headlines/get.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_latest_headlines/get.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_latest_headlines/post.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_latest_headlines/post.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_latest_headlines/post.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_latest_headlines/post.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search/get.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search/get.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,14 +197,15 @@
 ContentSentimentMinSchema = schemas.NumberSchema
 ContentSentimentMaxSchema = schemas.NumberSchema
 IptcTagsSchema = schemas.AnyTypeSchema
 NotIptcTagsSchema = schemas.AnyTypeSchema
 SourceNameSchema = schemas.AnyTypeSchema
 IabTagsSchema = schemas.AnyTypeSchema
 NotIabTagsSchema = schemas.AnyTypeSchema
+ExcludeDuplicatesSchema = schemas.BoolSchema
 RequestRequiredQueryParams = typing_extensions.TypedDict(
     'RequestRequiredQueryParams',
     {
         'q': typing.Union[QSchema, str, ],
     }
 )
 RequestOptionalQueryParams = typing_extensions.TypedDict(
@@ -252,14 +253,15 @@
         'content_sentiment_min': typing.Union[ContentSentimentMinSchema, decimal.Decimal, int, float, ],
         'content_sentiment_max': typing.Union[ContentSentimentMaxSchema, decimal.Decimal, int, float, ],
         'iptc_tags': typing.Union[IptcTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         'not_iptc_tags': typing.Union[NotIptcTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         'source_name': typing.Union[SourceNameSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         'iab_tags': typing.Union[IabTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         'not_iab_tags': typing.Union[NotIabTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        'exclude_duplicates': typing.Union[ExcludeDuplicatesSchema, bool, ],
     },
     total=False
 )
 
 
 class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
@@ -544,14 +546,20 @@
 )
 request_query_not_iab_tags = api_client.QueryParameter(
     name="not_iab_tags",
     style=api_client.ParameterStyle.FORM,
     schema=NotIabTagsSchema,
     explode=True,
 )
+request_query_exclude_duplicates = api_client.QueryParameter(
+    name="exclude_duplicates",
+    style=api_client.ParameterStyle.FORM,
+    schema=ExcludeDuplicatesSchema,
+    explode=True,
+)
 _auth = [
     'apiKey',
 ]
 SchemaFor200ResponseBodyApplicationJson = SearchGetResponseSchema
 
 
 @dataclass
@@ -649,14 +657,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _query_params = {}
         if q is not None:
             _query_params["q"] = q
         if search_in is not None:
             _query_params["search_in"] = search_in
@@ -746,14 +755,16 @@
             _query_params["not_iptc_tags"] = not_iptc_tags
         if source_name is not None:
             _query_params["source_name"] = source_name
         if iab_tags is not None:
             _query_params["iab_tags"] = iab_tags
         if not_iab_tags is not None:
             _query_params["not_iab_tags"] = not_iab_tags
+        if exclude_duplicates is not None:
+            _query_params["exclude_duplicates"] = exclude_duplicates
         args.query = _query_params
         return args
 
     async def _aget_oapg(
         self,
             query_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
@@ -820,14 +831,15 @@
             request_query_content_sentiment_min,
             request_query_content_sentiment_max,
             request_query_iptc_tags,
             request_query_not_iptc_tags,
             request_query_source_name,
             request_query_iab_tags,
             request_query_not_iab_tags,
+            request_query_exclude_duplicates,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -978,14 +990,15 @@
             request_query_content_sentiment_min,
             request_query_content_sentiment_max,
             request_query_iptc_tags,
             request_query_not_iptc_tags,
             request_query_source_name,
             request_query_iab_tags,
             request_query_not_iab_tags,
+            request_query_exclude_duplicates,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -1088,14 +1101,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._get_mapped_args(
@@ -1142,14 +1156,15 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
             not_iab_tags=not_iab_tags,
+            exclude_duplicates=exclude_duplicates,
         )
         return await self._aget_oapg(
             query_params=args.query,
             **kwargs,
         )
     
     def get(
@@ -1197,14 +1212,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._get_mapped_args(
             q=q,
             search_in=search_in,
@@ -1249,14 +1265,15 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
             not_iab_tags=not_iab_tags,
+            exclude_duplicates=exclude_duplicates,
         )
         return self._get_oapg(
             query_params=args.query,
         )
 
 class Get(BaseApi):
 
@@ -1305,14 +1322,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
         validate: bool = False,
         **kwargs,
     ) -> SearchGetResponsePydantic:
         raw_response = await self.raw.aget(
             q=q,
             search_in=search_in,
             predefined_sources=predefined_sources,
@@ -1356,14 +1374,15 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
             not_iab_tags=not_iab_tags,
+            exclude_duplicates=exclude_duplicates,
             **kwargs,
         )
         if validate:
             return RootModel[SearchGetResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(SearchGetResponsePydantic, raw_response.body)
     
     
@@ -1412,14 +1431,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
         validate: bool = False,
     ) -> SearchGetResponsePydantic:
         raw_response = self.raw.get(
             q=q,
             search_in=search_in,
             predefined_sources=predefined_sources,
             sources=sources,
@@ -1462,14 +1482,15 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
             not_iab_tags=not_iab_tags,
+            exclude_duplicates=exclude_duplicates,
         )
         if validate:
             return RootModel[SearchGetResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(SearchGetResponsePydantic, raw_response.body)
 
 
 class ApiForget(BaseApi):
@@ -1520,14 +1541,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._get_mapped_args(
@@ -1574,14 +1596,15 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
             not_iab_tags=not_iab_tags,
+            exclude_duplicates=exclude_duplicates,
         )
         return await self._aget_oapg(
             query_params=args.query,
             **kwargs,
         )
     
     def get(
@@ -1629,14 +1652,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._get_mapped_args(
             q=q,
             search_in=search_in,
@@ -1681,12 +1705,13 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
             not_iab_tags=not_iab_tags,
+            exclude_duplicates=exclude_duplicates,
         )
         return self._get_oapg(
             query_params=args.query,
         )
```

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search/get.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search/get.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -183,14 +183,15 @@
 ContentSentimentMinSchema = schemas.NumberSchema
 ContentSentimentMaxSchema = schemas.NumberSchema
 IptcTagsSchema = schemas.AnyTypeSchema
 NotIptcTagsSchema = schemas.AnyTypeSchema
 SourceNameSchema = schemas.AnyTypeSchema
 IabTagsSchema = schemas.AnyTypeSchema
 NotIabTagsSchema = schemas.AnyTypeSchema
+ExcludeDuplicatesSchema = schemas.BoolSchema
 RequestRequiredQueryParams = typing_extensions.TypedDict(
     'RequestRequiredQueryParams',
     {
         'q': typing.Union[QSchema, str, ],
     }
 )
 RequestOptionalQueryParams = typing_extensions.TypedDict(
@@ -238,14 +239,15 @@
         'content_sentiment_min': typing.Union[ContentSentimentMinSchema, decimal.Decimal, int, float, ],
         'content_sentiment_max': typing.Union[ContentSentimentMaxSchema, decimal.Decimal, int, float, ],
         'iptc_tags': typing.Union[IptcTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         'not_iptc_tags': typing.Union[NotIptcTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         'source_name': typing.Union[SourceNameSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         'iab_tags': typing.Union[IabTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         'not_iab_tags': typing.Union[NotIabTagsSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        'exclude_duplicates': typing.Union[ExcludeDuplicatesSchema, bool, ],
     },
     total=False
 )
 
 
 class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
@@ -530,14 +532,20 @@
 )
 request_query_not_iab_tags = api_client.QueryParameter(
     name="not_iab_tags",
     style=api_client.ParameterStyle.FORM,
     schema=NotIabTagsSchema,
     explode=True,
 )
+request_query_exclude_duplicates = api_client.QueryParameter(
+    name="exclude_duplicates",
+    style=api_client.ParameterStyle.FORM,
+    schema=ExcludeDuplicatesSchema,
+    explode=True,
+)
 SchemaFor200ResponseBodyApplicationJson = SearchGetResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     body: SearchGetResponse
 
@@ -628,14 +636,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _query_params = {}
         if q is not None:
             _query_params["q"] = q
         if search_in is not None:
             _query_params["search_in"] = search_in
@@ -725,14 +734,16 @@
             _query_params["not_iptc_tags"] = not_iptc_tags
         if source_name is not None:
             _query_params["source_name"] = source_name
         if iab_tags is not None:
             _query_params["iab_tags"] = iab_tags
         if not_iab_tags is not None:
             _query_params["not_iab_tags"] = not_iab_tags
+        if exclude_duplicates is not None:
+            _query_params["exclude_duplicates"] = exclude_duplicates
         args.query = _query_params
         return args
 
     async def _aget_oapg(
         self,
             query_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
@@ -799,14 +810,15 @@
             request_query_content_sentiment_min,
             request_query_content_sentiment_max,
             request_query_iptc_tags,
             request_query_not_iptc_tags,
             request_query_source_name,
             request_query_iab_tags,
             request_query_not_iab_tags,
+            request_query_exclude_duplicates,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -957,14 +969,15 @@
             request_query_content_sentiment_min,
             request_query_content_sentiment_max,
             request_query_iptc_tags,
             request_query_not_iptc_tags,
             request_query_source_name,
             request_query_iab_tags,
             request_query_not_iab_tags,
+            request_query_exclude_duplicates,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -1067,14 +1080,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._get_mapped_args(
@@ -1121,14 +1135,15 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
             not_iab_tags=not_iab_tags,
+            exclude_duplicates=exclude_duplicates,
         )
         return await self._aget_oapg(
             query_params=args.query,
             **kwargs,
         )
     
     def get(
@@ -1176,14 +1191,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._get_mapped_args(
             q=q,
             search_in=search_in,
@@ -1228,14 +1244,15 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
             not_iab_tags=not_iab_tags,
+            exclude_duplicates=exclude_duplicates,
         )
         return self._get_oapg(
             query_params=args.query,
         )
 
 class Get(BaseApi):
 
@@ -1284,14 +1301,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
         validate: bool = False,
         **kwargs,
     ) -> SearchGetResponsePydantic:
         raw_response = await self.raw.aget(
             q=q,
             search_in=search_in,
             predefined_sources=predefined_sources,
@@ -1335,14 +1353,15 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
             not_iab_tags=not_iab_tags,
+            exclude_duplicates=exclude_duplicates,
             **kwargs,
         )
         if validate:
             return RootModel[SearchGetResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(SearchGetResponsePydantic, raw_response.body)
     
     
@@ -1391,14 +1410,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
         validate: bool = False,
     ) -> SearchGetResponsePydantic:
         raw_response = self.raw.get(
             q=q,
             search_in=search_in,
             predefined_sources=predefined_sources,
             sources=sources,
@@ -1441,14 +1461,15 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
             not_iab_tags=not_iab_tags,
+            exclude_duplicates=exclude_duplicates,
         )
         if validate:
             return RootModel[SearchGetResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(SearchGetResponsePydantic, raw_response.body)
 
 
 class ApiForget(BaseApi):
@@ -1499,14 +1520,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._get_mapped_args(
@@ -1553,14 +1575,15 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
             not_iab_tags=not_iab_tags,
+            exclude_duplicates=exclude_duplicates,
         )
         return await self._aget_oapg(
             query_params=args.query,
             **kwargs,
         )
     
     def get(
@@ -1608,14 +1631,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._get_mapped_args(
             q=q,
             search_in=search_in,
@@ -1660,12 +1684,13 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
             not_iab_tags=not_iab_tags,
+            exclude_duplicates=exclude_duplicates,
         )
         return self._get_oapg(
             query_params=args.query,
         )
```

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search/post.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search/post.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,14 +160,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _body = {}
         if q is not None:
             _body["q"] = q
         if search_in is not None:
             _body["search_in"] = search_in
@@ -257,14 +258,16 @@
             _body["not_iptc_tags"] = not_iptc_tags
         if source_name is not None:
             _body["source_name"] = source_name
         if iab_tags is not None:
             _body["iab_tags"] = iab_tags
         if not_iab_tags is not None:
             _body["not_iab_tags"] = not_iab_tags
+        if exclude_duplicates is not None:
+            _body["exclude_duplicates"] = exclude_duplicates
         args.body = _body
         return args
 
     async def _apost_oapg(
         self,
         body: typing.Any = None,
         skip_deserialization: bool = True,
@@ -511,14 +514,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._post_mapped_args(
@@ -565,14 +569,15 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
             not_iab_tags=not_iab_tags,
+            exclude_duplicates=exclude_duplicates,
         )
         return await self._apost_oapg(
             body=args.body,
             **kwargs,
         )
     
     def post(
@@ -620,14 +625,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post_mapped_args(
             q=q,
             search_in=search_in,
@@ -672,14 +678,15 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
             not_iab_tags=not_iab_tags,
+            exclude_duplicates=exclude_duplicates,
         )
         return self._post_oapg(
             body=args.body,
         )
 
 class Post(BaseApi):
 
@@ -728,14 +735,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
         validate: bool = False,
         **kwargs,
     ) -> SearchPostResponsePydantic:
         raw_response = await self.raw.apost(
             q=q,
             search_in=search_in,
             predefined_sources=predefined_sources,
@@ -779,14 +787,15 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
             not_iab_tags=not_iab_tags,
+            exclude_duplicates=exclude_duplicates,
             **kwargs,
         )
         if validate:
             return RootModel[SearchPostResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(SearchPostResponsePydantic, raw_response.body)
     
     
@@ -835,14 +844,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
         validate: bool = False,
     ) -> SearchPostResponsePydantic:
         raw_response = self.raw.post(
             q=q,
             search_in=search_in,
             predefined_sources=predefined_sources,
             sources=sources,
@@ -885,14 +895,15 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
             not_iab_tags=not_iab_tags,
+            exclude_duplicates=exclude_duplicates,
         )
         if validate:
             return RootModel[SearchPostResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(SearchPostResponsePydantic, raw_response.body)
 
 
 class ApiForpost(BaseApi):
@@ -943,14 +954,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._post_mapped_args(
@@ -997,14 +1009,15 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
             not_iab_tags=not_iab_tags,
+            exclude_duplicates=exclude_duplicates,
         )
         return await self._apost_oapg(
             body=args.body,
             **kwargs,
         )
     
     def post(
@@ -1052,14 +1065,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post_mapped_args(
             q=q,
             search_in=search_in,
@@ -1104,12 +1118,13 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
             not_iab_tags=not_iab_tags,
+            exclude_duplicates=exclude_duplicates,
         )
         return self._post_oapg(
             body=args.body,
         )
```

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search/post.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search/post.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _body = {}
         if q is not None:
             _body["q"] = q
         if search_in is not None:
             _body["search_in"] = search_in
@@ -248,14 +249,16 @@
             _body["not_iptc_tags"] = not_iptc_tags
         if source_name is not None:
             _body["source_name"] = source_name
         if iab_tags is not None:
             _body["iab_tags"] = iab_tags
         if not_iab_tags is not None:
             _body["not_iab_tags"] = not_iab_tags
+        if exclude_duplicates is not None:
+            _body["exclude_duplicates"] = exclude_duplicates
         args.body = _body
         return args
 
     async def _apost_oapg(
         self,
         body: typing.Any = None,
         skip_deserialization: bool = True,
@@ -502,14 +505,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._post_mapped_args(
@@ -556,14 +560,15 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
             not_iab_tags=not_iab_tags,
+            exclude_duplicates=exclude_duplicates,
         )
         return await self._apost_oapg(
             body=args.body,
             **kwargs,
         )
     
     def post(
@@ -611,14 +616,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post_mapped_args(
             q=q,
             search_in=search_in,
@@ -663,14 +669,15 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
             not_iab_tags=not_iab_tags,
+            exclude_duplicates=exclude_duplicates,
         )
         return self._post_oapg(
             body=args.body,
         )
 
 class Post(BaseApi):
 
@@ -719,14 +726,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
         validate: bool = False,
         **kwargs,
     ) -> SearchPostResponsePydantic:
         raw_response = await self.raw.apost(
             q=q,
             search_in=search_in,
             predefined_sources=predefined_sources,
@@ -770,14 +778,15 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
             not_iab_tags=not_iab_tags,
+            exclude_duplicates=exclude_duplicates,
             **kwargs,
         )
         if validate:
             return RootModel[SearchPostResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(SearchPostResponsePydantic, raw_response.body)
     
     
@@ -826,14 +835,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
         validate: bool = False,
     ) -> SearchPostResponsePydantic:
         raw_response = self.raw.post(
             q=q,
             search_in=search_in,
             predefined_sources=predefined_sources,
             sources=sources,
@@ -876,14 +886,15 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
             not_iab_tags=not_iab_tags,
+            exclude_duplicates=exclude_duplicates,
         )
         if validate:
             return RootModel[SearchPostResponsePydantic](raw_response.body).root
         return api_client.construct_model_instance(SearchPostResponsePydantic, raw_response.body)
 
 
 class ApiForpost(BaseApi):
@@ -934,14 +945,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._post_mapped_args(
@@ -988,14 +1000,15 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
             not_iab_tags=not_iab_tags,
+            exclude_duplicates=exclude_duplicates,
         )
         return await self._apost_oapg(
             body=args.body,
             **kwargs,
         )
     
     def post(
@@ -1043,14 +1056,15 @@
         content_sentiment_min: typing.Optional[typing.Union[int, float]] = None,
         content_sentiment_max: typing.Optional[typing.Union[int, float]] = None,
         iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iptc_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
         not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = None,
+        exclude_duplicates: typing.Optional[bool] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._post_mapped_args(
             q=q,
             search_in=search_in,
@@ -1095,12 +1109,13 @@
             content_sentiment_min=content_sentiment_min,
             content_sentiment_max=content_sentiment_max,
             iptc_tags=iptc_tags,
             not_iptc_tags=not_iptc_tags,
             source_name=source_name,
             iab_tags=iab_tags,
             not_iab_tags=not_iab_tags,
+            exclude_duplicates=exclude_duplicates,
         )
         return self._post_oapg(
             body=args.body,
         )
```

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_by_link/get.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_by_link/get.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_by_link/get.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_by_link/get.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_by_link/post.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_by_link/post.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_by_link/post.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_by_link/post.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_similar/get.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_similar/get.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_similar/get.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_similar/get.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_similar/post.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_similar/post.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_search_similar/post.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_search_similar/post.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_sources/get.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_sources/get.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_sources/get.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_sources/get.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_sources/post.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_sources/post.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_sources/post.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_sources/post.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_subscription/get.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_subscription/get.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_subscription/get.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_subscription/get.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_subscription/post.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_subscription/post.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/paths/api_subscription/post.pyi` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/paths/api_subscription/post.pyi`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/additional_source_info.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/additional_source_info.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/author_search_request.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/author_search_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/authors_get_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/authors_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/authors_post_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/authors_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/cluster.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/cluster.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/cluster_articles.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/cluster_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/clustering_search_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/clustering_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_author_search_response_article_result.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_author_search_response_article_result.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_author_search_response_failed_search_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_author_search_response_failed_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_author_search_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_article_result.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_article_result.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_failed_search_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_failed_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_more_like_this_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_search_response_search_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_search_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/dto_responses_search_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/dto_responses_search_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/http_validation_error.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/latest_headlines_get_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/latest_headlines_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/latest_headlines_post_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/latest_headlines_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/latest_headlines_request.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/latest_headlines_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/latest_headlines_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/latest_headlines_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/latest_headlines_response_articles.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/latest_headlines_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/more_like_this_request.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/more_like_this_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/search_get_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/search_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/search_post_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/search_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/search_request.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/search_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,11 +108,13 @@
 
     source_name: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = Field(None, alias='source_name')
 
     iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = Field(None, alias='iab_tags')
 
     not_iab_tags: typing.Optional[typing.Union[bool, date, datetime, dict, float, int, list, str, None]] = Field(None, alias='not_iab_tags')
 
+    exclude_duplicates: typing.Optional[bool] = Field(None, alias='exclude_duplicates')
+
     model_config = ConfigDict(
         protected_namespaces=(),
         arbitrary_types_allowed=True
     )
```

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/search_similar_get_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/search_similar_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/search_similar_post_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/search_similar_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/search_url_request.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/search_url_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/similar_document.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/similar_document.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/source_info.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/source_info.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/source_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/source_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/source_response_sources.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/source_response_sources.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/sources_request.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/sources_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/subscription_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/subscription_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/validation_error.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/validation_error.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/pydantic/validation_error_loc.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/pydantic/validation_error_loc.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/request_after_hook.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/request_after_hook.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/request_before_hook.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/request_before_hook.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/request_before_url_hook.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/request_before_url_hook.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/rest.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/schemas.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/schemas.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/additional_source_info.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/additional_source_info.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/author_search_request.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/author_search_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/authors_get_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/authors_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/authors_post_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/authors_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/cluster.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/cluster.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/cluster_articles.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/cluster_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/clustering_search_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/clustering_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_author_search_response_article_result.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_author_search_response_article_result.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_author_search_response_failed_search_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_author_search_response_failed_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_author_search_response_search_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_author_search_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_author_search_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_author_search_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_more_like_this_response_article_result.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_more_like_this_response_article_result.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_more_like_this_response_failed_search_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_more_like_this_response_failed_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_more_like_this_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_search_response_search_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_search_response_search_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/dto_responses_search_response_search_response_articles.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/dto_responses_search_response_search_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/http_validation_error.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/latest_headlines_get_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/latest_headlines_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/latest_headlines_post_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/latest_headlines_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/latest_headlines_request.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/latest_headlines_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/latest_headlines_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/latest_headlines_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/latest_headlines_response_articles.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/latest_headlines_response_articles.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/more_like_this_request.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/more_like_this_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/search_get_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/search_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/search_post_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/search_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/search_request.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/search_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,9 +108,11 @@
 
     source_name: typing.Union[bool, date, datetime, dict, float, int, list, str, None]
 
     iab_tags: typing.Union[bool, date, datetime, dict, float, int, list, str, None]
 
     not_iab_tags: typing.Union[bool, date, datetime, dict, float, int, list, str, None]
 
+    exclude_duplicates: bool
+
 class SearchRequest(RequiredSearchRequest, OptionalSearchRequest):
     pass
```

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/search_similar_get_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/search_similar_get_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/search_similar_post_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/search_similar_post_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/search_url_request.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/search_url_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/similar_document.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/similar_document.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/source_info.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/source_info.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/source_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/source_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/source_response_sources.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/source_response_sources.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/sources_request.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/sources_request.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/subscription_response.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/subscription_response.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/validation_error.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/validation_error.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type/validation_error_loc.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type/validation_error_loc.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/type_util.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/type_util.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/newscatcherapi_client/validation_metadata.py` & `newscatcherapi_python_sdk-6.0.5/newscatcherapi_client/validation_metadata.py`

 * *Files identical despite different names*

### Comparing `newscatcherapi_python_sdk-6.0.4/pyproject.toml` & `newscatcherapi_python_sdk-6.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "newscatcherapi-python-sdk"
-version = "6.0.4"
+version = "6.0.5"
 description = "Client for NewsCatcher-V3 Production API"
 authors = ["Maksym Sugonyaka <maksym@newscatcherapi.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "newscatcherapi_client"}]
 
 [tool.poetry.dependencies]
```

### Comparing `newscatcherapi_python_sdk-6.0.4/PKG-INFO` & `newscatcherapi_python_sdk-6.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,13 @@
-Metadata-Version: 2.1
-Name: newscatcherapi-python-sdk
-Version: 6.0.4
-Summary: Client for NewsCatcher-V3 Production API
-License: MIT
-Author: Maksym Sugonyaka
-Author-email: maksym@newscatcherapi.com
-Requires-Python: >=3.7,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: certifi (>=2023.7.22)
-Requires-Dist: cryptography (>=42.0.5,<43.0.0)
-Requires-Dist: frozendict (>=2.3.4,<3.0.0)
-Requires-Dist: pydantic (>=2.4.2,<3.0.0)
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: typing_extensions (>=4.3.0,<5.0.0)
-Requires-Dist: urllib3 (>=1.26.18,<2.0.0)
-Description-Content-Type: text/markdown
-
 # newscatcherapi-python-sdk<a id="newscatcherapi-python-sdk"></a>
 
 <img src='https://uploads-ssl.webflow.com/6429857b17973b636c2195c5/646c6f1eb774ff2f2997bec5_newscatcher_.svg' width='286' height='35' /> <br>  <br>Visit our website  <a href='https://newscatcherapi.com'>https://newscatcherapi.com</a>
 
 
-[![PyPI](https://img.shields.io/badge/PyPI-v6.0.4-blue)](https://pypi.org/project/newscatcherapi-python-sdk/6.0.4)
+[![PyPI](https://img.shields.io/badge/PyPI-v6.0.5-blue)](https://pypi.org/project/newscatcherapi-python-sdk/6.0.5)
 [![README.md](https://img.shields.io/badge/README-Click%20Here-green)](https://github.com/konfig-dev/newscatcher-sdks/tree/main/v3/python#readme)
 
 ## Table of Contents<a id="table-of-contents"></a>
 
 <!-- toc -->
 
 - [Requirements](#requirements)
@@ -52,25 +26,27 @@
   * [`newscatcher.search_link.post`](#newscatchersearch_linkpost)
   * [`newscatcher.search_similar.get`](#newscatchersearch_similarget)
   * [`newscatcher.search_similar.post`](#newscatchersearch_similarpost)
   * [`newscatcher.sources.get`](#newscatchersourcesget)
   * [`newscatcher.sources.post`](#newscatchersourcespost)
   * [`newscatcher.subscription.get`](#newscatchersubscriptionget)
   * [`newscatcher.subscription.post`](#newscatchersubscriptionpost)
+  * [`newscatcher.search_duplicates_by_original_id.get`](#newscatchersearch_duplicates_by_original_idget)
+  * [`newscatcher.search_duplicates_by_original_id.post`](#newscatchersearch_duplicates_by_original_idpost)
 
 <!-- tocstop -->
 
 ## Requirements<a id="requirements"></a>
 
 Python >=3.7
 
 ## Installation<a id="installation"></a>
 
 ```sh
-pip install newscatcherapi-python-sdk==6.0.4
+pip install newscatcherapi-python-sdk==6.0.5
 ```
 
 ## Getting Started<a id="getting-started"></a>
 
 ```python
 from pprint import pprint
 from newscatcherapi_client import Newscatcher, ApiException
@@ -908,14 +884,15 @@
     content_sentiment_min=3.14,
     content_sentiment_max=3.14,
     iptc_tags=None,
     not_iptc_tags=None,
     source_name=None,
     iab_tags=None,
     not_iab_tags=None,
+    exclude_duplicates=True,
 )
 ```
 
 #### ⚙️ Parameters<a id="⚙️-parameters"></a>
 
 ##### q: `str`<a id="q-str"></a>
 
@@ -1009,14 +986,16 @@
 
 ##### source_name: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="source_name-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
 
 ##### iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
 
 ##### not_iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/.py)<a id="not_iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypepy"></a>
 
+##### exclude_duplicates: `bool`<a id="exclude_duplicates-bool"></a>
+
 #### 🔄 Return<a id="🔄-return"></a>
 
 [`SearchGetResponse`](./newscatcherapi_client/pydantic/search_get_response.py)
 
 #### 🌐 Endpoint<a id="🌐-endpoint"></a>
 
 `/api/search` `get`
@@ -1076,14 +1055,15 @@
     content_sentiment_min=3.14,
     content_sentiment_max=3.14,
     iptc_tags=None,
     not_iptc_tags=None,
     source_name=None,
     iab_tags=None,
     not_iab_tags=None,
+    exclude_duplicates=True,
 )
 ```
 
 #### ⚙️ Parameters<a id="⚙️-parameters"></a>
 
 ##### q: `str`<a id="q-str"></a>
 
@@ -1177,14 +1157,16 @@
 
 ##### source_name: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="source_name-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
 
 ##### iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
 
 ##### not_iab_tags: [`Union[bool, date, datetime, dict, float, int, list, str, None]`](./newscatcherapi_client/type/typing_union_bool_date_datetime_dict_float_int_list_str_none.py)<a id="not_iab_tags-unionbool-date-datetime-dict-float-int-list-str-nonenewscatcherapi_clienttypetyping_union_bool_date_datetime_dict_float_int_list_str_nonepy"></a>
 
+##### exclude_duplicates: `bool`<a id="exclude_duplicates-bool"></a>
+
 #### ⚙️ Request Body<a id="⚙️-request-body"></a>
 
 [`SearchRequest`](./newscatcherapi_client/type/search_request.py)
 #### 🔄 Return<a id="🔄-return"></a>
 
 [`SearchPostResponse`](./newscatcherapi_client/pydantic/search_post_response.py)
 
@@ -1711,11 +1693,81 @@
 
 `/api/subscription` `post`
 
 [🔙 **Back to Table of Contents**](#table-of-contents)
 
 ---
 
+### `newscatcher.search_duplicates_by_original_id.get`<a id="newscatchersearch_duplicates_by_original_idget"></a>
+
+This endpoint allows you to search for duplicate articles by original article id.
+
+#### 🛠️ Usage<a id="🛠️-usage"></a>
+
+```python
+get_response = newscatcher.search_duplicates_by_original_id.get(
+    original_article_id="original_article_id_example",
+    page=1,
+    page_size=100,
+)
+```
+
+#### ⚙️ Parameters<a id="⚙️-parameters"></a>
+
+##### original_article_id: `str`<a id="original_article_id-str"></a>
+
+##### page: `int`<a id="page-int"></a>
+
+##### page_size: `int`<a id="page_size-int"></a>
+
+#### 🔄 Return<a id="🔄-return"></a>
+
+[`SearchduplicatesbyoriginalidGetResponse`](./newscatcherapi_client/pydantic/searchduplicatesbyoriginalid_get_response.py)
+
+#### 🌐 Endpoint<a id="🌐-endpoint"></a>
+
+`/api/search_duplicates_by_original_id` `get`
+
+[🔙 **Back to Table of Contents**](#table-of-contents)
+
+---
+
+### `newscatcher.search_duplicates_by_original_id.post`<a id="newscatchersearch_duplicates_by_original_idpost"></a>
+
+This endpoint allows you to search for duplicate articles by original article id.
+
+#### 🛠️ Usage<a id="🛠️-usage"></a>
+
+```python
+post_response = newscatcher.search_duplicates_by_original_id.post(
+    original_article_id="string_example",
+    page=1,
+    page_size=100,
+)
+```
+
+#### ⚙️ Parameters<a id="⚙️-parameters"></a>
+
+##### original_article_id: `str`<a id="original_article_id-str"></a>
+
+##### page: `int`<a id="page-int"></a>
+
+##### page_size: `int`<a id="page_size-int"></a>
+
+#### ⚙️ Request Body<a id="⚙️-request-body"></a>
+
+[`DuplicatesByOriginalIdRequest`](./newscatcherapi_client/type/duplicates_by_original_id_request.py)
+#### 🔄 Return<a id="🔄-return"></a>
+
+[`SearchduplicatesbyoriginalidPostResponse`](./newscatcherapi_client/pydantic/searchduplicatesbyoriginalid_post_response.py)
+
+#### 🌐 Endpoint<a id="🌐-endpoint"></a>
+
+`/api/search_duplicates_by_original_id` `post`
+
+[🔙 **Back to Table of Contents**](#table-of-contents)
+
+---
+
 
 ## Author<a id="author"></a>
 This Python package is automatically generated by [Konfig](https://konfigthis.com)
-
```

