# Comparing `tmp/social-auth-core-4.5.3.tar.gz` & `tmp/social-auth-core-4.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "social-auth-core-4.5.3.tar", last modified: Wed Feb 14 10:21:19 2024, max compression
+gzip compressed data, was "social-auth-core-4.5.4.tar", last modified: Thu Apr 25 07:05:04 2024, max compression
```

## Comparing `social-auth-core-4.5.3.tar` & `social-auth-core-4.5.4.tar`

### file list

```diff
@@ -1,384 +1,384 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 10:21:19.538302 social-auth-core-4.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)    20714 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-02-14 10:21:19.538302 social-auth-core-4.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/requirements-azuread.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/requirements-base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/requirements-saml.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-14 10:21:19.538302 social-auth-core-4.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 10:21:19.482303 social-auth-core-4.5.3/social_auth_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-02-14 10:21:19.000000 social-auth-core-4.5.3/social_auth_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13467 2024-02-14 10:21:19.000000 social-auth-core-4.5.3/social_auth_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 10:21:19.000000 social-auth-core-4.5.3/social_auth_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 10:21:19.000000 social-auth-core-4.5.3/social_auth_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-02-14 10:21:19.000000 social-auth-core-4.5.3/social_auth_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-14 10:21:19.000000 social-auth-core-4.5.3/social_auth_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 10:21:19.482303 social-auth-core-4.5.3/social_core/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 10:21:19.514302 social-auth-core-4.5.3/social_core/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/amazon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/angel.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/aol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/apple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/appsfuel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/arcgis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/asana.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/atlassian.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/auth0.py
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/azuread.py
--rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/azuread_b2c.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/azuread_tenant.py
--rw-r--r--   0 runner    (1001) docker     (127)    10137 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/battlenet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/beats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/behance.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/belgiumeid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/bitbucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/bitbucket_datacenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/bungie.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/cas.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/changetip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/chatwork.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/cilogon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/classlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/clef.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/clever.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/coding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/cognito.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/coinbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/coursera.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/dailymotion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/deezer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/digitalocean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/discogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/discord.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/discourse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/disqus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/douban.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/dribbble.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/drip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/dropbox.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/echosign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/edmodo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/egi_checkin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/einfracz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/elixir.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/etsy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/eventbrite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/eveonline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/evernote.py
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/exacttarget.py
--rw-r--r--   0 runner    (1001) docker     (127)     8975 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/facebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/facebook_limited.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/fedora.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/fence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/fitbit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/five_hundred_px.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/flat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/flickr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/foursquare.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/gae.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/gitea.py
--rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/github_enterprise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/globus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/goclio.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/goclioeu.py
--rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/google.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/google_openidconnect.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/grafana.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/hubspot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/instagram.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/itembase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/jawbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/justgiving.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/kakao.py
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/keycloak.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/khanacademy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/lastfm.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/launchpad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/linkedin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/live.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/livejournal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/loginradius.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/lyft.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/mailchimp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/mailru.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/mapmyfitness.py
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/mediawiki.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/meetup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/mendeley.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/microsoft.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/mineid.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/mixcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/monzo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/moves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/musicbrainz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/nationbuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/naver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/ngpvan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/nk.py
--rw-r--r--   0 runner    (1001) docker     (127)    19366 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/odnoklassniki.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/okta.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/okta_openidconnect.py
--rw-r--r--   0 runner    (1001) docker     (127)     9982 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/open_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    10138 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/open_id_connect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/openinfra.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/openshift.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/openstack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/openstreetmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/openstreetmap_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/orbi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/orcid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/osso.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/patreon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/paypal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/persona.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/phabricator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/pinterest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/pixelpin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/pocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/podio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/professionali.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/pushbullet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/qiita.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/qq.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/quizlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/rdio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/readability.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/reddit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/runkeeper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/salesforce.py
--rw-r--r--   0 runner    (1001) docker     (127)    14883 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/saml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/scistarter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/seznam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/shimmering.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/shopify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/simplelogin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/sketchfab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/skyrock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/slack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/soundcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/spotify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/stackoverflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/steam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/stocktwits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/strava.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/stripe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/surveymonkey.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/suse.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/taobao.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/telegram.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/thisismyjam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/trello.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/tripit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/tumblr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/twilio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/twitch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/twitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/twitter_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/uber.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/ubuntu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/udata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/uffd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/universe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/untappd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/upwork.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/username.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/vault.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/vend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/vimeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/vk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/weibo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/weixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/withings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/wlcg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/wunderlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/xing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/yahoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/yammer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/yandex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/backends/zotero.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 10:21:19.514302 social-auth-core-4.5.3/social_core/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/pipeline/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/pipeline/disconnect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/pipeline/mail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/pipeline/partial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/pipeline/social_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/pipeline/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/pipeline/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10496 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/store.py
--rw-r--r--   0 runner    (1001) docker     (127)     8613 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 10:21:19.518302 social-auth-core-4.5.3/social_core/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 10:21:19.518302 social-auth-core-4.5.3/social_core/tests/actions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8690 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/actions/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/actions/test_associate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/actions/test_disconnect.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/actions/test_login.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 10:21:19.538302 social-auth-core-4.5.3/social_core/tests/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 10:21:19.538302 social-auth-core-4.5.3/social_core/tests/backends/data/
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/data/saml_config.json
--rw-r--r--   0 runner    (1001) docker     (127)    17556 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/data/saml_response.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17495 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/data/saml_response_legacy.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17493 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/data/saml_response_no_idp_name.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17520 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/data/saml_response_no_next_url.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/open_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_amazon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_angel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_apple.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_arcgis.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_asana.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_atlassian.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_auth0.py
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_azuread.py
--rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_azuread_b2c.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_behance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_bitbucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_bitbucket_datacenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_box.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_broken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_cas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_chatwork.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_cilogon.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_clef.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_cognito.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_coinbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_coursera.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_dailymotion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_deezer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_digitalocean.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_discogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_discourse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_disqus.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_dribbble.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_drip.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_dropbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_edmodo.py
--rw-r--r--   0 runner    (1001) docker     (127)    10362 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_egi_checkin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_einfracz.py
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_elixir.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_etsy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_eventbrite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_evernote.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_facebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_fence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_fitbit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_five_hundred_px.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_flat.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_flickr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_foursquare.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_gitea.py
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_github.py
--rw-r--r--   0 runner    (1001) docker     (127)    10862 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_github_enterprise.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_gitlab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_globus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_google.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_grafana.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_instagram.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_itembase.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_kakao.py
--rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_keycloak.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_khanacademy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_linkedin.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_live.py
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_livejournal.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_lyft.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_mailru.py
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_mapmyfitness.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_microsoft.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_mineid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_mixcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_musicbrainz.py
--rw-r--r--   0 runner    (1001) docker     (127)     9263 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_nationbuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_naver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8634 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_ngpvan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_okta.py
--rw-r--r--   0 runner    (1001) docker     (127)     9855 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_open_id_connect.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_openstreetmap_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_orbi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_orcid.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_osso.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_patreon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_paypal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_phabricator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_pinterest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_podio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_qiita.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_quizlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_readability.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_reddit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_scistarter.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_seznam.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_simplelogin.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_sketchfab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_skyrock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_slack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_soundcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_spotify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_stackoverflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_steam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_stocktwits.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_strava.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_stripe.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_taobao.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_thisismyjam.py
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_tripit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_tumblr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_twitch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9766 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_twitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_twitter_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_uber.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_udata.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_universe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_upwork.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_username.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_vault.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_vk.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_wlcg.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_wunderlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_xing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_yahoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_yammer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_yandex.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/backends/test_zotero.py
--rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/test_partial.py
--rw-r--r--   0 runner    (1001) docker     (127)     8685 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/tests/testkey.pem
--rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-02-14 10:21:10.000000 social-auth-core-4.5.3/social_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:05:04.348502 social-auth-core-4.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    21024 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-25 07:05:04.348502 social-auth-core-4.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/requirements-azuread.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/requirements-base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/requirements-saml.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-25 07:05:04.348502 social-auth-core-4.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:05:04.296502 social-auth-core-4.5.4/social_auth_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-25 07:05:04.000000 social-auth-core-4.5.4/social_auth_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13467 2024-04-25 07:05:04.000000 social-auth-core-4.5.4/social_auth_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 07:05:04.000000 social-auth-core-4.5.4/social_auth_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 07:05:04.000000 social-auth-core-4.5.4/social_auth_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-25 07:05:04.000000 social-auth-core-4.5.4/social_auth_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 07:05:04.000000 social-auth-core-4.5.4/social_auth_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:05:04.296502 social-auth-core-4.5.4/social_core/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:05:04.324502 social-auth-core-4.5.4/social_core/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/amazon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/angel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/aol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/apple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/appsfuel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/arcgis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/asana.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/atlassian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/auth0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/azuread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/azuread_b2c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/azuread_tenant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10133 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/battlenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/beats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/behance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/belgiumeid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/bitbucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/bitbucket_datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/bungie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/cas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/changetip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/chatwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/cilogon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/classlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/clef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/clever.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/coding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/cognito.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/coinbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/coursera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/dailymotion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/deezer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/digitalocean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/discogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/discord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/discourse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/disqus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/douban.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/dribbble.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/drip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/echosign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/edmodo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/egi_checkin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/einfracz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/elixir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/etsy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/eventbrite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/eveonline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/evernote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/exacttarget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8975 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/facebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/facebook_limited.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/fedora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/fence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/fitbit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/five_hundred_px.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/flickr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/foursquare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/gae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/gitea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/github_enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/globus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/goclio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/goclioeu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/google_openidconnect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/grafana.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/hubspot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/instagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/itembase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/jawbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/justgiving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/kakao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/keycloak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/khanacademy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/lastfm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/launchpad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/linkedin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/live.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/livejournal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/loginradius.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/lyft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/mailchimp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/mailru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/mapmyfitness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/mediawiki.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/meetup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/mendeley.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/microsoft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/mineid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/mixcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/monzo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/moves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/musicbrainz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/nationbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/naver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/ngpvan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/nk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19366 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/odnoklassniki.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/okta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/okta_openidconnect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9982 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/open_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10138 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/open_id_connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/openinfra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/openshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/openstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/openstreetmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/openstreetmap_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/orbi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/orcid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/osso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/patreon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/paypal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/persona.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/phabricator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/pinterest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/pixelpin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/pocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/podio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/professionali.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/pushbullet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/qiita.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/qq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/quizlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/rdio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/readability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/runkeeper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/salesforce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14883 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/scistarter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/seznam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/shimmering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/shopify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/simplelogin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/sketchfab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/skyrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/slack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/soundcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/spotify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/stackoverflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/steam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/stocktwits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/strava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/stripe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/surveymonkey.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/suse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/taobao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/thisismyjam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/trello.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/tripit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/tumblr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/twilio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/twitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/twitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/twitter_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/uber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/ubuntu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/udata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/uffd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/universe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/untappd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/upwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/username.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/vault.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/vend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/vimeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/vk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/weibo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/weixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/withings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/wlcg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/wunderlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/xing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/yahoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/yammer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/yandex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/backends/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:05:04.328502 social-auth-core-4.5.4/social_core/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/pipeline/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/pipeline/disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/pipeline/mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/pipeline/partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/pipeline/social_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/pipeline/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/pipeline/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10496 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8613 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:05:04.328502 social-auth-core-4.5.4/social_core/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:05:04.328502 social-auth-core-4.5.4/social_core/tests/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8690 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/actions/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/actions/test_associate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/actions/test_disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/actions/test_login.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:05:04.348502 social-auth-core-4.5.4/social_core/tests/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:05:04.348502 social-auth-core-4.5.4/social_core/tests/backends/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/data/saml_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17556 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/data/saml_response.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17495 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/data/saml_response_legacy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17493 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/data/saml_response_no_idp_name.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17520 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/data/saml_response_no_next_url.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/open_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_amazon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_angel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_apple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_arcgis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_asana.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_atlassian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_auth0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_azuread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_azuread_b2c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_behance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_bitbucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_bitbucket_datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_broken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_cas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_chatwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_cilogon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_clef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_cognito.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_coinbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_coursera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_dailymotion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_deezer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_digitalocean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_discogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_discourse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_disqus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_dribbble.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_drip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_edmodo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10362 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_egi_checkin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_einfracz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_elixir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_etsy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_eventbrite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_evernote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_facebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_fence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_fitbit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_five_hundred_px.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_flickr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_foursquare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_gitea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10862 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_github_enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_globus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_grafana.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_instagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_itembase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_kakao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_keycloak.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_khanacademy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_linkedin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_live.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_livejournal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_lyft.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_mailru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_mapmyfitness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_microsoft.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_mineid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_mixcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_musicbrainz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9263 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_nationbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_naver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8634 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_ngpvan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_okta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9855 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_open_id_connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_openstreetmap_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_orbi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_orcid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_osso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_patreon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_paypal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_phabricator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_pinterest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_podio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_qiita.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_quizlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_readability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_reddit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_scistarter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_seznam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_simplelogin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_sketchfab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_skyrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_slack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_soundcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_spotify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_stackoverflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_steam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_stocktwits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_strava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_stripe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_taobao.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_thisismyjam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_tripit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_tumblr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_twitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9766 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_twitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_twitter_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_uber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_udata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_universe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_upwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_username.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_vault.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_vk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_wlcg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_wunderlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_xing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_yahoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_yammer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_yandex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/backends/test_zotero.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/test_partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8685 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/tests/testkey.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-04-25 07:04:54.000000 social-auth-core-4.5.4/social_core/utils.py
```

### Comparing `social-auth-core-4.5.3/CHANGELOG.md` & `social-auth-core-4.5.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 # Change Log
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/).
 
+## [4.5.4](https://github.com/python-social-auth/social-core/releases/tag/4.5.4) - 2024-04-25
+
+### Added
+- LinkedIn supports refresh token
+
+### Changed
+- SteamOpenId validation of identify URL
+- Box state redirestion
+- The `uid` is automatically converted to string in the pipeline
+- Mediawiki error handling
+
 ## [4.5.3](https://github.com/python-social-auth/social-core/releases/tag/4.5.3) - 2024-02-14
 
 ### Added
 - OpenStreetMap OAuth2
 
 ### Changed
 - Etsy backend fixes
```

### Comparing `social-auth-core-4.5.3/LICENSE` & `social-auth-core-4.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/PKG-INFO` & `social-auth-core-4.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: social-auth-core
-Version: 4.5.3
+Version: 4.5.4
 Summary: Python social authentication made simple.
 Home-page: https://github.com/python-social-auth/social-core
 Author: Matias Aguirre
 Author-email: matiasaguirre@gmail.com
 License: BSD
 Keywords: openid,oauth,saml,social auth
 Platform: UNKNOWN
```

### Comparing `social-auth-core-4.5.3/README.md` & `social-auth-core-4.5.4/README.md`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/setup.py` & `social-auth-core-4.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_auth_core.egg-info/PKG-INFO` & `social-auth-core-4.5.4/social_auth_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: social-auth-core
-Version: 4.5.3
+Version: 4.5.4
 Summary: Python social authentication made simple.
 Home-page: https://github.com/python-social-auth/social-core
 Author: Matias Aguirre
 Author-email: matiasaguirre@gmail.com
 License: BSD
 Keywords: openid,oauth,saml,social auth
 Platform: UNKNOWN
```

### Comparing `social-auth-core-4.5.3/social_auth_core.egg-info/SOURCES.txt` & `social-auth-core-4.5.4/social_auth_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/actions.py` & `social-auth-core-4.5.4/social_core/actions.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/amazon.py` & `social-auth-core-4.5.4/social_core/backends/amazon.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/angel.py` & `social-auth-core-4.5.4/social_core/backends/angel.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/apple.py` & `social-auth-core-4.5.4/social_core/backends/apple.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/appsfuel.py` & `social-auth-core-4.5.4/social_core/backends/appsfuel.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/arcgis.py` & `social-auth-core-4.5.4/social_core/backends/arcgis.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/asana.py` & `social-auth-core-4.5.4/social_core/backends/asana.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/atlassian.py` & `social-auth-core-4.5.4/social_core/backends/atlassian.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/auth0.py` & `social-auth-core-4.5.4/social_core/backends/auth0.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/azuread.py` & `social-auth-core-4.5.4/social_core/backends/azuread.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/azuread_b2c.py` & `social-auth-core-4.5.4/social_core/backends/azuread_b2c.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/azuread_tenant.py` & `social-auth-core-4.5.4/social_core/backends/azuread_tenant.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/base.py` & `social-auth-core-4.5.4/social_core/backends/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
                 if size == 3:
                     name, alias, discard = entry
                 elif size == 2:
                     (name, alias), discard = entry, False
                 elif size == 1:
                     name = alias = entry[0]
                     discard = False
-                value = response.get(name) or details.get(name) or details.get(alias)
+                value = response.get(name, details.get(name, details.get(alias)))
                 if discard and not value:
                     continue
                 data[alias] = value
         return data
 
     def auth_allowed(self, response, details):
         """Return True if the user should be allowed to authenticate, by
```

### Comparing `social-auth-core-4.5.3/social_core/backends/battlenet.py` & `social-auth-core-4.5.4/social_core/backends/battlenet.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/beats.py` & `social-auth-core-4.5.4/social_core/backends/beats.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/behance.py` & `social-auth-core-4.5.4/social_core/backends/behance.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/bitbucket.py` & `social-auth-core-4.5.4/social_core/backends/bitbucket.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/bitbucket_datacenter.py` & `social-auth-core-4.5.4/social_core/backends/bitbucket_datacenter.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/box.py` & `social-auth-core-4.5.4/social_core/backends/box.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
     name = "box"
     AUTHORIZATION_URL = "https://www.box.com/api/oauth2/authorize"
     ACCESS_TOKEN_METHOD = "POST"
     ACCESS_TOKEN_URL = "https://www.box.com/api/oauth2/token"
     REVOKE_TOKEN_URL = "https://www.box.com/api/oauth2/revoke"
     SCOPE_SEPARATOR = ","
+    REDIRECT_STATE = False
     EXTRA_DATA = [
         ("refresh_token", "refresh_token", True),
         ("id", "id"),
         ("expires", "expires"),
     ]
 
     def do_auth(self, access_token, response=None, *args, **kwargs):
```

### Comparing `social-auth-core-4.5.3/social_core/backends/bungie.py` & `social-auth-core-4.5.4/social_core/backends/bungie.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/cas.py` & `social-auth-core-4.5.4/social_core/backends/cas.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/changetip.py` & `social-auth-core-4.5.4/social_core/backends/changetip.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/chatwork.py` & `social-auth-core-4.5.4/social_core/backends/chatwork.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/cilogon.py` & `social-auth-core-4.5.4/social_core/backends/cilogon.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/classlink.py` & `social-auth-core-4.5.4/social_core/backends/classlink.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/clef.py` & `social-auth-core-4.5.4/social_core/backends/clef.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/clever.py` & `social-auth-core-4.5.4/social_core/backends/clever.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/coding.py` & `social-auth-core-4.5.4/social_core/backends/coding.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/cognito.py` & `social-auth-core-4.5.4/social_core/backends/cognito.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/coinbase.py` & `social-auth-core-4.5.4/social_core/backends/coinbase.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/coursera.py` & `social-auth-core-4.5.4/social_core/backends/coursera.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/dailymotion.py` & `social-auth-core-4.5.4/social_core/backends/dailymotion.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/deezer.py` & `social-auth-core-4.5.4/social_core/backends/deezer.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/digitalocean.py` & `social-auth-core-4.5.4/social_core/backends/digitalocean.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/discogs.py` & `social-auth-core-4.5.4/social_core/backends/discogs.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/discord.py` & `social-auth-core-4.5.4/social_core/backends/discord.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/discourse.py` & `social-auth-core-4.5.4/social_core/backends/discourse.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/disqus.py` & `social-auth-core-4.5.4/social_core/backends/disqus.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/docker.py` & `social-auth-core-4.5.4/social_core/backends/docker.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/douban.py` & `social-auth-core-4.5.4/social_core/backends/douban.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/dribbble.py` & `social-auth-core-4.5.4/social_core/backends/dribbble.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/drip.py` & `social-auth-core-4.5.4/social_core/backends/drip.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/dropbox.py` & `social-auth-core-4.5.4/social_core/backends/dropbox.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/echosign.py` & `social-auth-core-4.5.4/social_core/backends/echosign.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/edmodo.py` & `social-auth-core-4.5.4/social_core/backends/edmodo.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/egi_checkin.py` & `social-auth-core-4.5.4/social_core/backends/egi_checkin.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/einfracz.py` & `social-auth-core-4.5.4/social_core/backends/einfracz.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/elixir.py` & `social-auth-core-4.5.4/social_core/backends/elixir.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/etsy.py` & `social-auth-core-4.5.4/social_core/backends/etsy.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/eventbrite.py` & `social-auth-core-4.5.4/social_core/backends/eventbrite.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/eveonline.py` & `social-auth-core-4.5.4/social_core/backends/eveonline.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/evernote.py` & `social-auth-core-4.5.4/social_core/backends/evernote.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/exacttarget.py` & `social-auth-core-4.5.4/social_core/backends/exacttarget.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/facebook.py` & `social-auth-core-4.5.4/social_core/backends/facebook.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/facebook_limited.py` & `social-auth-core-4.5.4/social_core/backends/facebook_limited.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/fence.py` & `social-auth-core-4.5.4/social_core/backends/fence.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/fitbit.py` & `social-auth-core-4.5.4/social_core/backends/fitbit.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/five_hundred_px.py` & `social-auth-core-4.5.4/social_core/backends/five_hundred_px.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/flat.py` & `social-auth-core-4.5.4/social_core/backends/flat.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/flickr.py` & `social-auth-core-4.5.4/social_core/backends/flickr.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/foursquare.py` & `social-auth-core-4.5.4/social_core/backends/foursquare.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/gae.py` & `social-auth-core-4.5.4/social_core/backends/gae.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/gitea.py` & `social-auth-core-4.5.4/social_core/backends/gitea.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/github.py` & `social-auth-core-4.5.4/social_core/backends/github.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/github_enterprise.py` & `social-auth-core-4.5.4/social_core/backends/github_enterprise.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/gitlab.py` & `social-auth-core-4.5.4/social_core/backends/gitlab.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/globus.py` & `social-auth-core-4.5.4/social_core/backends/globus.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/goclio.py` & `social-auth-core-4.5.4/social_core/backends/goclio.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/google.py` & `social-auth-core-4.5.4/social_core/backends/google.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/google_openidconnect.py` & `social-auth-core-4.5.4/social_core/backends/google_openidconnect.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/grafana.py` & `social-auth-core-4.5.4/social_core/backends/grafana.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/hubspot.py` & `social-auth-core-4.5.4/social_core/backends/hubspot.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/instagram.py` & `social-auth-core-4.5.4/social_core/backends/instagram.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/itembase.py` & `social-auth-core-4.5.4/social_core/backends/itembase.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/jawbone.py` & `social-auth-core-4.5.4/social_core/backends/jawbone.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/justgiving.py` & `social-auth-core-4.5.4/social_core/backends/justgiving.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/kakao.py` & `social-auth-core-4.5.4/social_core/backends/kakao.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/keycloak.py` & `social-auth-core-4.5.4/social_core/backends/keycloak.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/khanacademy.py` & `social-auth-core-4.5.4/social_core/backends/khanacademy.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/lastfm.py` & `social-auth-core-4.5.4/social_core/backends/lastfm.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/legacy.py` & `social-auth-core-4.5.4/social_core/backends/legacy.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/line.py` & `social-auth-core-4.5.4/social_core/backends/line.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/linkedin.py` & `social-auth-core-4.5.4/social_core/backends/linkedin.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,14 +57,16 @@
     REDIRECT_STATE = False
     DEFAULT_SCOPE = ["r_liteprofile"]
     EXTRA_DATA = [
         ("id", "id"),
         ("expires_in", "expires"),
         ("firstName", "first_name"),
         ("lastName", "last_name"),
+        ("refresh_token", "refresh_token"),
+        ("refresh_token_expires_in", "refresh_expires_in"),
     ]
 
     def user_details_url(self):
         # use set() since LinkedIn fails when values are duplicated
         fields_selectors = list(
             set(["id", "firstName", "lastName"] + self.setting("FIELD_SELECTORS", []))
         )
```

### Comparing `social-auth-core-4.5.3/social_core/backends/live.py` & `social-auth-core-4.5.4/social_core/backends/live.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/livejournal.py` & `social-auth-core-4.5.4/social_core/backends/livejournal.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/loginradius.py` & `social-auth-core-4.5.4/social_core/backends/loginradius.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/lyft.py` & `social-auth-core-4.5.4/social_core/backends/lyft.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/mailchimp.py` & `social-auth-core-4.5.4/social_core/backends/mailchimp.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/mailru.py` & `social-auth-core-4.5.4/social_core/backends/mailru.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/mapmyfitness.py` & `social-auth-core-4.5.4/social_core/backends/mapmyfitness.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/mediawiki.py` & `social-auth-core-4.5.4/social_core/backends/mediawiki.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,16 @@
         auth_token = self.oauth_auth(token)
 
         response = requests.post(
             url=self.setting("MEDIAWIKI_URL"),
             params={"title": "Special:Oauth/token"},
             auth=auth_token,
         )
+        if response.content.decode().startswith("Error"):
+            raise AuthException(self, response.content.decode())
         credentials = parse_qs(response.content)
         oauth_token_key = credentials.get(b"oauth_token")[0]
         oauth_token_secret = credentials.get(b"oauth_token_secret")[0]
         oauth_token_key = oauth_token_key.decode()
         oauth_token_secret = oauth_token_secret.decode()
 
         return {
```

### Comparing `social-auth-core-4.5.3/social_core/backends/meetup.py` & `social-auth-core-4.5.4/social_core/backends/meetup.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/mendeley.py` & `social-auth-core-4.5.4/social_core/backends/mendeley.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/microsoft.py` & `social-auth-core-4.5.4/social_core/backends/microsoft.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/mineid.py` & `social-auth-core-4.5.4/social_core/backends/mineid.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/mixcloud.py` & `social-auth-core-4.5.4/social_core/backends/mixcloud.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/monzo.py` & `social-auth-core-4.5.4/social_core/backends/monzo.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/moves.py` & `social-auth-core-4.5.4/social_core/backends/moves.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/musicbrainz.py` & `social-auth-core-4.5.4/social_core/backends/musicbrainz.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/nationbuilder.py` & `social-auth-core-4.5.4/social_core/backends/nationbuilder.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/naver.py` & `social-auth-core-4.5.4/social_core/backends/naver.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/ngpvan.py` & `social-auth-core-4.5.4/social_core/backends/ngpvan.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/nk.py` & `social-auth-core-4.5.4/social_core/backends/nk.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/oauth.py` & `social-auth-core-4.5.4/social_core/backends/oauth.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/odnoklassniki.py` & `social-auth-core-4.5.4/social_core/backends/odnoklassniki.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/okta.py` & `social-auth-core-4.5.4/social_core/backends/okta.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/open_id.py` & `social-auth-core-4.5.4/social_core/backends/open_id.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/open_id_connect.py` & `social-auth-core-4.5.4/social_core/backends/open_id_connect.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/openinfra.py` & `social-auth-core-4.5.4/social_core/backends/openinfra.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/openshift.py` & `social-auth-core-4.5.4/social_core/backends/openshift.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/openstack.py` & `social-auth-core-4.5.4/social_core/backends/openstack.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/openstreetmap.py` & `social-auth-core-4.5.4/social_core/backends/openstreetmap.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/openstreetmap_oauth2.py` & `social-auth-core-4.5.4/social_core/backends/openstreetmap_oauth2.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/orbi.py` & `social-auth-core-4.5.4/social_core/backends/orbi.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/orcid.py` & `social-auth-core-4.5.4/social_core/backends/orcid.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/osso.py` & `social-auth-core-4.5.4/social_core/backends/osso.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/patreon.py` & `social-auth-core-4.5.4/social_core/backends/patreon.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/paypal.py` & `social-auth-core-4.5.4/social_core/backends/paypal.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/persona.py` & `social-auth-core-4.5.4/social_core/backends/persona.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/phabricator.py` & `social-auth-core-4.5.4/social_core/backends/phabricator.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/ping.py` & `social-auth-core-4.5.4/social_core/backends/ping.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/pinterest.py` & `social-auth-core-4.5.4/social_core/backends/pinterest.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/pixelpin.py` & `social-auth-core-4.5.4/social_core/backends/pixelpin.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/pocket.py` & `social-auth-core-4.5.4/social_core/backends/pocket.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/podio.py` & `social-auth-core-4.5.4/social_core/backends/podio.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/professionali.py` & `social-auth-core-4.5.4/social_core/backends/professionali.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/pushbullet.py` & `social-auth-core-4.5.4/social_core/backends/pushbullet.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/qiita.py` & `social-auth-core-4.5.4/social_core/backends/qiita.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/qq.py` & `social-auth-core-4.5.4/social_core/backends/qq.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/quizlet.py` & `social-auth-core-4.5.4/social_core/backends/quizlet.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/rdio.py` & `social-auth-core-4.5.4/social_core/backends/rdio.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/readability.py` & `social-auth-core-4.5.4/social_core/backends/readability.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/reddit.py` & `social-auth-core-4.5.4/social_core/backends/reddit.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/runkeeper.py` & `social-auth-core-4.5.4/social_core/backends/runkeeper.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/salesforce.py` & `social-auth-core-4.5.4/social_core/backends/salesforce.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/saml.py` & `social-auth-core-4.5.4/social_core/backends/saml.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/scistarter.py` & `social-auth-core-4.5.4/social_core/backends/scistarter.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/seznam.py` & `social-auth-core-4.5.4/social_core/backends/seznam.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/shimmering.py` & `social-auth-core-4.5.4/social_core/backends/shimmering.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/shopify.py` & `social-auth-core-4.5.4/social_core/backends/shopify.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/simplelogin.py` & `social-auth-core-4.5.4/social_core/backends/simplelogin.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/sketchfab.py` & `social-auth-core-4.5.4/social_core/backends/sketchfab.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/skyrock.py` & `social-auth-core-4.5.4/social_core/backends/skyrock.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/slack.py` & `social-auth-core-4.5.4/social_core/backends/slack.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/soundcloud.py` & `social-auth-core-4.5.4/social_core/backends/soundcloud.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/spotify.py` & `social-auth-core-4.5.4/social_core/backends/spotify.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/stackoverflow.py` & `social-auth-core-4.5.4/social_core/backends/stackoverflow.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/steam.py` & `social-auth-core-4.5.4/social_core/backends/steam.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,11 +42,13 @@
     def consumer(self):
         # Steam seems to support stateless mode only, ignore store
         if not hasattr(self, "_consumer"):
             self._consumer = self.create_consumer()
         return self._consumer
 
     def _user_id(self, response):
+        if not response.identity_url.startswith(self.URL):
+            raise AuthFailed(self, "Openid identifier mismatch")
         user_id = response.identity_url.rsplit("/", 1)[-1]
         if not user_id.isdigit():
             raise AuthFailed(self, "Missing Steam Id")
         return user_id
```

### Comparing `social-auth-core-4.5.3/social_core/backends/stocktwits.py` & `social-auth-core-4.5.4/social_core/backends/stocktwits.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/strava.py` & `social-auth-core-4.5.4/social_core/backends/strava.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/stripe.py` & `social-auth-core-4.5.4/social_core/backends/stripe.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/surveymonkey.py` & `social-auth-core-4.5.4/social_core/backends/surveymonkey.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/taobao.py` & `social-auth-core-4.5.4/social_core/backends/taobao.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/telegram.py` & `social-auth-core-4.5.4/social_core/backends/telegram.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/thisismyjam.py` & `social-auth-core-4.5.4/social_core/backends/thisismyjam.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/trello.py` & `social-auth-core-4.5.4/social_core/backends/trello.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/tripit.py` & `social-auth-core-4.5.4/social_core/backends/tripit.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/tumblr.py` & `social-auth-core-4.5.4/social_core/backends/tumblr.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/twilio.py` & `social-auth-core-4.5.4/social_core/backends/twilio.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/twitch.py` & `social-auth-core-4.5.4/social_core/backends/twitch.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/twitter.py` & `social-auth-core-4.5.4/social_core/backends/twitter.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/twitter_oauth2.py` & `social-auth-core-4.5.4/social_core/backends/twitter_oauth2.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/uber.py` & `social-auth-core-4.5.4/social_core/backends/uber.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/udata.py` & `social-auth-core-4.5.4/social_core/backends/udata.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/uffd.py` & `social-auth-core-4.5.4/social_core/backends/uffd.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/universe.py` & `social-auth-core-4.5.4/social_core/backends/universe.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/untappd.py` & `social-auth-core-4.5.4/social_core/backends/untappd.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/upwork.py` & `social-auth-core-4.5.4/social_core/backends/upwork.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/utils.py` & `social-auth-core-4.5.4/social_core/backends/utils.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/vend.py` & `social-auth-core-4.5.4/social_core/backends/vend.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/vimeo.py` & `social-auth-core-4.5.4/social_core/backends/vimeo.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/vk.py` & `social-auth-core-4.5.4/social_core/backends/vk.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/weibo.py` & `social-auth-core-4.5.4/social_core/backends/weibo.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/weixin.py` & `social-auth-core-4.5.4/social_core/backends/weixin.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/withings.py` & `social-auth-core-4.5.4/social_core/backends/withings.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/wlcg.py` & `social-auth-core-4.5.4/social_core/backends/wlcg.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/wunderlist.py` & `social-auth-core-4.5.4/social_core/backends/wunderlist.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/xing.py` & `social-auth-core-4.5.4/social_core/backends/xing.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/yahoo.py` & `social-auth-core-4.5.4/social_core/backends/yahoo.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/yammer.py` & `social-auth-core-4.5.4/social_core/backends/yammer.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/yandex.py` & `social-auth-core-4.5.4/social_core/backends/yandex.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/zoom.py` & `social-auth-core-4.5.4/social_core/backends/zoom.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/backends/zotero.py` & `social-auth-core-4.5.4/social_core/backends/zotero.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/exceptions.py` & `social-auth-core-4.5.4/social_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/pipeline/__init__.py` & `social-auth-core-4.5.4/social_core/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/pipeline/disconnect.py` & `social-auth-core-4.5.4/social_core/pipeline/disconnect.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/pipeline/mail.py` & `social-auth-core-4.5.4/social_core/pipeline/mail.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/pipeline/partial.py` & `social-auth-core-4.5.4/social_core/pipeline/partial.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/pipeline/social_auth.py` & `social-auth-core-4.5.4/social_core/pipeline/social_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 def social_details(backend, details, response, *args, **kwargs):
     return {"details": dict(backend.get_user_details(response), **details)}
 
 
 def social_uid(backend, details, response, *args, **kwargs):
-    return {"uid": backend.get_user_id(details, response)}
+    return {"uid": str(backend.get_user_id(details, response))}
 
 
 def auth_allowed(backend, details, response, *args, **kwargs):
     if not backend.auth_allowed(response, details):
         raise AuthForbidden(backend)
```

### Comparing `social-auth-core-4.5.3/social_core/pipeline/user.py` & `social-auth-core-4.5.4/social_core/pipeline/user.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/pipeline/utils.py` & `social-auth-core-4.5.4/social_core/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/storage.py` & `social-auth-core-4.5.4/social_core/storage.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/store.py` & `social-auth-core-4.5.4/social_core/store.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/strategy.py` & `social-auth-core-4.5.4/social_core/strategy.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/actions/actions.py` & `social-auth-core-4.5.4/social_core/tests/actions/actions.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/actions/test_associate.py` & `social-auth-core-4.5.4/social_core/tests/actions/test_associate.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/actions/test_disconnect.py` & `social-auth-core-4.5.4/social_core/tests/actions/test_disconnect.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/actions/test_login.py` & `social-auth-core-4.5.4/social_core/tests/actions/test_login.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/base.py` & `social-auth-core-4.5.4/social_core/tests/backends/base.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/data/saml_config.json` & `social-auth-core-4.5.4/social_core/tests/backends/data/saml_config.json`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/data/saml_response.txt` & `social-auth-core-4.5.4/social_core/tests/backends/data/saml_response.txt`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/data/saml_response_legacy.txt` & `social-auth-core-4.5.4/social_core/tests/backends/data/saml_response_legacy.txt`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/data/saml_response_no_idp_name.txt` & `social-auth-core-4.5.4/social_core/tests/backends/data/saml_response_no_idp_name.txt`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/data/saml_response_no_next_url.txt` & `social-auth-core-4.5.4/social_core/tests/backends/data/saml_response_no_next_url.txt`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/legacy.py` & `social-auth-core-4.5.4/social_core/tests/backends/legacy.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/oauth.py` & `social-auth-core-4.5.4/social_core/tests/backends/oauth.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/open_id.py` & `social-auth-core-4.5.4/social_core/tests/backends/open_id.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_amazon.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_amazon.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_angel.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_angel.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_apple.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_apple.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_arcgis.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_arcgis.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_asana.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_asana.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_atlassian.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_atlassian.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_auth0.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_auth0.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_azuread.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_azuread.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_azuread_b2c.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_azuread_b2c.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_behance.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_behance.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_bitbucket.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_bitbucket.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_bitbucket_datacenter.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_bitbucket_datacenter.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
     def test_login(self):
         user = self.do_login()
 
         self.assertEqual(len(user.social), 1)
 
         social = user.social[0]
-        self.assertEqual(social.uid, 1)
+        self.assertEqual(social.uid, "1")
         self.assertEqual(social.extra_data["first_name"], "Erlich")
         self.assertEqual(social.extra_data["last_name"], "Bachman")
         self.assertEqual(social.extra_data["email"], "erlich@bachmanity.com")
         self.assertEqual(social.extra_data["name"], "erlich-bachman")
         self.assertEqual(social.extra_data["username"], "erlich-bachman")
         self.assertEqual(social.extra_data["display_name"], "Erlich Bachman")
         self.assertEqual(social.extra_data["type"], "NORMAL")
@@ -105,15 +105,15 @@
         self.assertEqual(social.extra_data["token_type"], "bearer")
         self.assertEqual(social.extra_data["expires"], 3600)
         self.assertEqual(social.extra_data["refresh_token"], "dummy_refresh_token")
 
     def test_refresh_token(self):
         _, social = self.do_refresh_token()
 
-        self.assertEqual(social.uid, 1)
+        self.assertEqual(social.uid, "1")
         self.assertEqual(social.extra_data["first_name"], "Erlich")
         self.assertEqual(social.extra_data["last_name"], "Bachman")
         self.assertEqual(social.extra_data["email"], "erlich@bachmanity.com")
         self.assertEqual(social.extra_data["name"], "erlich-bachman")
         self.assertEqual(social.extra_data["username"], "erlich-bachman")
         self.assertEqual(social.extra_data["display_name"], "Erlich Bachman")
         self.assertEqual(social.extra_data["type"], "NORMAL")
```

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_box.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_box.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_broken.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_broken.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_cas.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_cas.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_chatwork.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_chatwork.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_cilogon.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_cilogon.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_clef.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_clef.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_cognito.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_cognito.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_coinbase.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_coinbase.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_coursera.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_coursera.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_dailymotion.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_dailymotion.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_deezer.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_deezer.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_digitalocean.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_digitalocean.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_discogs.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_discogs.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_discourse.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_discourse.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_disqus.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_disqus.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_dribbble.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_dribbble.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_drip.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_drip.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_dropbox.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_dropbox.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_dummy.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_dummy.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_edmodo.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_edmodo.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_egi_checkin.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_egi_checkin.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_einfracz.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_einfracz.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_elixir.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_elixir.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_etsy.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_etsy.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_eventbrite.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_eventbrite.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_evernote.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_evernote.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_facebook.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_facebook.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_fence.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_fence.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_fitbit.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_fitbit.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_five_hundred_px.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_five_hundred_px.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_flat.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_flat.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_flickr.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_flickr.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_foursquare.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_foursquare.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_gitea.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_gitea.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_github.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_github.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_github_enterprise.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_github_enterprise.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_gitlab.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_globus.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_globus.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_google.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_google.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_grafana.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_grafana.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_instagram.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_instagram.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_itembase.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_itembase.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_kakao.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_kakao.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_keycloak.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_keycloak.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_khanacademy.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_khanacademy.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_linkedin.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_linkedin.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_live.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_live.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_livejournal.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_livejournal.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_lyft.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_lyft.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_mailru.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_mailru.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_mapmyfitness.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_mapmyfitness.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_microsoft.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_microsoft.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_mineid.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_mineid.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_mixcloud.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_mixcloud.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_musicbrainz.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_musicbrainz.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_nationbuilder.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_nationbuilder.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_naver.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_naver.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_ngpvan.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_ngpvan.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_okta.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_okta.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_open_id_connect.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_open_id_connect.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_openstreetmap_oauth2.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_openstreetmap_oauth2.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_orbi.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_orbi.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_orcid.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_orcid.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_osso.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_osso.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_patreon.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_patreon.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_paypal.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_paypal.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_phabricator.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_phabricator.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_pinterest.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_pinterest.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_podio.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_podio.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_qiita.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_qiita.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_quizlet.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_quizlet.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_readability.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_readability.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_reddit.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_reddit.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_saml.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_saml.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_scistarter.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_scistarter.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_seznam.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_seznam.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_simplelogin.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_simplelogin.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_sketchfab.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_sketchfab.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_skyrock.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_skyrock.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_slack.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_slack.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_soundcloud.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_soundcloud.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_spotify.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_spotify.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_stackoverflow.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_stackoverflow.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_steam.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_steam.py`

 * *Files 25% similar despite different names*

```diff
@@ -136,7 +136,37 @@
         with self.assertRaises(AuthFailed):
             self.do_login()
 
     def test_partial_pipeline(self):
         self._login_setup(user_url="https://steamcommunity.com/openid/BROKEN")
         with self.assertRaises(AuthFailed):
             self.do_partial_pipeline()
+
+
+class SteamOpenIdFakeSteamIdTest(SteamOpenIdTest):
+    server_response = urlencode(
+        {
+            "janrain_nonce": JANRAIN_NONCE,
+            "openid.ns": "http://specs.openid.net/auth/2.0",
+            "openid.mode": "id_res",
+            "openid.op_endpoint": "https://steamcommunity.com/openid/login",
+            "openid.claimed_id": "https://fakesteamcommunity.com/openid/123",
+            "openid.identity": "https://fakesteamcommunity.com/openid/123",
+            "openid.return_to": "http://myapp.com/complete/steam/?"
+            "janrain_nonce=" + JANRAIN_NONCE,
+            "openid.response_nonce": JANRAIN_NONCE + "oD4UZ3w9chOAiQXk0AqDipqFYRA=",
+            "openid.assoc_handle": "1234567890",
+            "openid.signed": "signed,op_endpoint,claimed_id,identity,return_to,"
+            "response_nonce,assoc_handle",
+            "openid.sig": "1az53vj9SVdiBwhk8%2BFQ68R2plo=",
+        }
+    )
+
+    def test_login(self):
+        self._login_setup(user_url="https://fakesteamcommunity.com/openid/123")
+        with self.assertRaises(AuthFailed):
+            self.do_login()
+
+    def test_partial_pipeline(self):
+        self._login_setup(user_url="https://fakesteamcommunity.com/openid/123")
+        with self.assertRaises(AuthFailed):
+            self.do_partial_pipeline()
```

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_stocktwits.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_stocktwits.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_strava.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_strava.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_stripe.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_stripe.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_taobao.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_taobao.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_thisismyjam.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_thisismyjam.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_tripit.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_tripit.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_tumblr.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_tumblr.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_twitch.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_twitch.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_twitter.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_twitter.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_twitter_oauth2.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_twitter_oauth2.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_uber.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_uber.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_udata.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_udata.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_universe.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_universe.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_upwork.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_upwork.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_utils.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_utils.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_vault.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_vault.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_vk.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_vk.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_wlcg.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_wlcg.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_wunderlist.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_wunderlist.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_xing.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_xing.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_yahoo.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_yahoo.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_yammer.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_yammer.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_yandex.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_yandex.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_zoom.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_zoom.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/backends/test_zotero.py` & `social-auth-core-4.5.4/social_core/tests/backends/test_zotero.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/models.py` & `social-auth-core-4.5.4/social_core/tests/models.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/pipeline.py` & `social-auth-core-4.5.4/social_core/tests/pipeline.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/strategy.py` & `social-auth-core-4.5.4/social_core/tests/strategy.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/test_exceptions.py` & `social-auth-core-4.5.4/social_core/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/test_partial.py` & `social-auth-core-4.5.4/social_core/tests/test_partial.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/test_pipeline.py` & `social-auth-core-4.5.4/social_core/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/test_storage.py` & `social-auth-core-4.5.4/social_core/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/test_utils.py` & `social-auth-core-4.5.4/social_core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/tests/testkey.pem` & `social-auth-core-4.5.4/social_core/tests/testkey.pem`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.5.3/social_core/utils.py` & `social-auth-core-4.5.4/social_core/utils.py`

 * *Files identical despite different names*

