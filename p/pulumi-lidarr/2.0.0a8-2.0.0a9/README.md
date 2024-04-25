# Comparing `tmp/pulumi_lidarr-2.0.0a8.tar.gz` & `tmp/pulumi_lidarr-2.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_lidarr-2.0.0a8.tar", last modified: Wed Apr 24 16:24:22 2024, max compression
+gzip compressed data, was "pulumi_lidarr-2.0.0a9.tar", last modified: Thu Apr 25 16:29:10 2024, max compression
```

## Comparing `pulumi_lidarr-2.0.0a8.tar` & `pulumi_lidarr-2.0.0a9.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:24:22.619994 pulumi_lidarr-2.0.0a8/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-24 16:24:22.619994 pulumi_lidarr-2.0.0a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:24:22.591994 pulumi_lidarr-2.0.0a8/pulumi_lidarr/
--rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9369 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:24:22.591994 pulumi_lidarr-2.0.0a8/pulumi_lidarr/artists/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/artists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20858 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/artists/artist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7224 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/artists/get_artist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/artists/get_artists.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/artists/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:24:22.591994 pulumi_lidarr-2.0.0a8/pulumi_lidarr/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:24:22.595994 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23990 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/aria2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10804 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    34406 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/deluge.py
--rw-r--r--   0 runner    (1001) docker     (127)    84761 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/download_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    36251 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/flood.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    24033 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/get_download_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/get_download_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/get_remote_path_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/get_remote_path_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)    27437 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/hadouken.py
--rw-r--r--   0 runner    (1001) docker     (127)    34558 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/nzbget.py
--rw-r--r--   0 runner    (1001) docker     (127)    28900 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/nzbvortex.py
--rw-r--r--   0 runner    (1001) docker     (127)    16667 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19751 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/pneumatic.py
--rw-r--r--   0 runner    (1001) docker     (127)    40680 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/qbittorrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/remote_path_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    38316 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/rtorrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    34447 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/sabnzbd.py
--rw-r--r--   0 runner    (1001) docker     (127)    26221 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/torrent_blackhole.py
--rw-r--r--   0 runner    (1001) docker     (127)    28199 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/torrent_download_station.py
--rw-r--r--   0 runner    (1001) docker     (127)    35867 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/transmission.py
--rw-r--r--   0 runner    (1001) docker     (127)    20047 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/usenet_blackhole.py
--rw-r--r--   0 runner    (1001) docker     (127)    28167 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/usenet_download_station.py
--rw-r--r--   0 runner    (1001) docker     (127)    36637 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/utorrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    35579 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/vuze.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:24:22.599994 pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/exclusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/get_exclusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/get_exclusions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15913 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/get_import_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/get_import_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)    30385 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/headphones.py
--rw-r--r--   0 runner    (1001) docker     (127)    56058 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/import_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    30318 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/lastfm_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    30396 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/lastfm_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    34565 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/lidarr.py
--rw-r--r--   0 runner    (1001) docker     (127)    28444 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/lidarr_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    28610 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/music_brainz.py
--rw-r--r--   0 runner    (1001) docker     (127)    10780 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    32483 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/spotify_albums.py
--rw-r--r--   0 runner    (1001) docker     (127)    32539 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/spotify_artists.py
--rw-r--r--   0 runner    (1001) docker     (127)    34905 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/spotify_playlists.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:24:22.603994 pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27973 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/filelist.py
--rw-r--r--   0 runner    (1001) docker     (127)    32303 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/gazelle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    17698 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/get_indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/get_indexers.py
--rw-r--r--   0 runner    (1001) docker     (127)    24260 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/headphones.py
--rw-r--r--   0 runner    (1001) docker     (127)    61747 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)    18621 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/iptorrents.py
--rw-r--r--   0 runner    (1001) docker     (127)    25484 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/newznab.py
--rw-r--r--   0 runner    (1001) docker     (127)    25302 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/nyaa.py
--rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    29107 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/redacted.py
--rw-r--r--   0 runner    (1001) docker     (127)    21527 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/torrent_rss.py
--rw-r--r--   0 runner    (1001) docker     (127)    26692 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/torrentleech.py
--rw-r--r--   0 runner    (1001) docker     (127)    30132 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/torznab.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:24:22.603994 pulumi_lidarr-2.0.0a8/pulumi_lidarr/mediamanagement/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/mediamanagement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13362 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/mediamanagement/get_media_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/mediamanagement/get_naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/mediamanagement/get_root_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/mediamanagement/get_root_folders.py
--rw-r--r--   0 runner    (1001) docker     (127)    47165 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/mediamanagement/media_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    16798 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/mediamanagement/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/mediamanagement/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19452 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/mediamanagement/root_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:24:22.607994 pulumi_lidarr-2.0.0a8/pulumi_lidarr/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10560 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/metadata/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/metadata/get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/metadata/get_consumers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/metadata/get_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    17534 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/metadata/kodi.py
--rw-r--r--   0 runner    (1001) docker     (127)    23491 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/metadata/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15631 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/metadata/roksbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    11521 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/metadata/wdtv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:24:22.611994 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44934 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/apprise.py
--rw-r--r--   0 runner    (1001) docker     (127)    37628 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/custom_script.py
--rw-r--r--   0 runner    (1001) docker     (127)    48258 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/discord.py
--rw-r--r--   0 runner    (1001) docker     (127)    44670 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/email.py
--rw-r--r--   0 runner    (1001) docker     (127)    39932 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/emby.py
--rw-r--r--   0 runner    (1001) docker     (127)    44622 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/get_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/get_notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)    34932 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/gotify.py
--rw-r--r--   0 runner    (1001) docker     (127)    32164 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/join.py
--rw-r--r--   0 runner    (1001) docker     (127)    43228 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/kodi.py
--rw-r--r--   0 runner    (1001) docker     (127)    35819 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/mailgun.py
--rw-r--r--   0 runner    (1001) docker     (127)    28297 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/notifiarr.py
--rw-r--r--   0 runner    (1001) docker     (127)   162903 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    43633 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/ntfy.py
--rw-r--r--   0 runner    (1001) docker     (127)    28889 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28145 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/plex.py
--rw-r--r--   0 runner    (1001) docker     (127)    30190 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/prowl.py
--rw-r--r--   0 runner    (1001) docker     (127)    38562 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/pushbullet.py
--rw-r--r--   0 runner    (1001) docker     (127)    41609 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/pushover.py
--rw-r--r--   0 runner    (1001) docker     (127)    36342 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/sendgrid.py
--rw-r--r--   0 runner    (1001) docker     (127)    43017 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)    33882 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/simplepush.py
--rw-r--r--   0 runner    (1001) docker     (127)    40840 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/slack.py
--rw-r--r--   0 runner    (1001) docker     (127)    39066 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/subsonic.py
--rw-r--r--   0 runner    (1001) docker     (127)    21947 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/synology_indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)    36166 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/telegram.py
--rw-r--r--   0 runner    (1001) docker     (127)    42644 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/twitter.py
--rw-r--r--   0 runner    (1001) docker     (127)    41015 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:24:22.615994 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13049 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/custom_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    18912 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/delay_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_condition_release_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_condition_release_title.py
--rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_condition_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_custom_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_custom_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_delay_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_delay_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_metadata_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_metadata_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_primary_album_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_primary_album_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_quality_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_quality_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_quality_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_quality_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_release_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_release_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_release_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_release_statuses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_secondary_album_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_secondary_album_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    13922 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/metadata_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    31419 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11489 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/quality_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    20734 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/quality_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    14271 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/release_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:24:22.619994 pulumi_lidarr-2.0.0a8/pulumi_lidarr/system/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/system/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/system/get_host.py
--rw-r--r--   0 runner    (1001) docker     (127)    17897 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/system/get_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    26639 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/system/host.py
--rw-r--r--   0 runner    (1001) docker     (127)    23157 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/system/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:24:22.619994 pulumi_lidarr-2.0.0a8/pulumi_lidarr/tags/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/tags/get_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/tags/get_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/tags/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr/tags/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:24:22.591994 pulumi_lidarr-2.0.0a8/pulumi_lidarr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/pulumi_lidarr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 16:24:22.619994 pulumi_lidarr-2.0.0a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-24 16:24:22.000000 pulumi_lidarr-2.0.0a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:10.834798 pulumi_lidarr-2.0.0a9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-25 16:29:10.834798 pulumi_lidarr-2.0.0a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:10.806798 pulumi_lidarr-2.0.0a9/pulumi_lidarr/
+-rw-r--r--   0 runner    (1001) docker     (127)    17013 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9369 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:10.810798 pulumi_lidarr-2.0.0a9/pulumi_lidarr/artists/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/artists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20858 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/artists/artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7224 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/artists/get_artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/artists/get_artists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/artists/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:10.810798 pulumi_lidarr-2.0.0a9/pulumi_lidarr/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:10.814798 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23990 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/aria2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10804 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34406 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/deluge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84761 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/download_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36251 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/flood.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24033 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/get_download_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/get_download_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/get_remote_path_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/get_remote_path_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27437 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/hadouken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34558 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/nzbget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28900 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/nzbvortex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16667 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19751 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/pneumatic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40680 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/qbittorrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/remote_path_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38316 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/rtorrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34447 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/sabnzbd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26221 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/torrent_blackhole.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28199 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/torrent_download_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35867 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/transmission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20047 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/usenet_blackhole.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28167 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/usenet_download_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36637 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/utorrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35579 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/vuze.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:10.818798 pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/exclusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/get_exclusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/get_exclusions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15913 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/get_import_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/get_import_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30385 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/headphones.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56058 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/import_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30318 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/lastfm_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30396 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/lastfm_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34565 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/lidarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28444 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/lidarr_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28610 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/music_brainz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10780 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32483 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/spotify_albums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32539 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/spotify_artists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34905 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/spotify_playlists.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:10.818798 pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27973 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/filelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32303 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/gazelle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17698 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/get_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/get_indexers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24260 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/headphones.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61747 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18621 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/iptorrents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25484 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/newznab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25302 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/nyaa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29107 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/redacted.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21527 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/torrent_rss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26692 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/torrentleech.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30132 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/torznab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:10.822798 pulumi_lidarr-2.0.0a9/pulumi_lidarr/mediamanagement/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/mediamanagement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13362 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/mediamanagement/get_media_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/mediamanagement/get_naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/mediamanagement/get_root_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/mediamanagement/get_root_folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47165 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/mediamanagement/media_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16798 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/mediamanagement/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/mediamanagement/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19452 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/mediamanagement/root_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:10.822798 pulumi_lidarr-2.0.0a9/pulumi_lidarr/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10560 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/metadata/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/metadata/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/metadata/get_consumers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/metadata/get_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/metadata/get_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/metadata/get_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17534 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/metadata/kodi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23491 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/metadata/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13714 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/metadata/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15631 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/metadata/roksbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11521 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/metadata/wdtv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:10.830798 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44934 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/apprise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37628 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/custom_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48258 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/discord.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44670 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39932 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/emby.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44622 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/get_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/get_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34932 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/gotify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32164 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43228 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/kodi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35819 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/mailgun.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28297 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/notifiarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)   162903 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43633 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/ntfy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28889 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28145 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/plex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30190 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/prowl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38562 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/pushbullet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41609 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/pushover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36342 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/sendgrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43017 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33882 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/simplepush.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40840 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/slack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39066 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/subsonic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21947 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/synology_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36166 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42644 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/twitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41015 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:10.834798 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13049 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/custom_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18912 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/delay_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_condition_release_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_condition_release_title.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_condition_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_custom_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_custom_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_delay_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_delay_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_primary_album_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_primary_album_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_release_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_release_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_release_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_release_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_secondary_album_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_secondary_album_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29204 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20314 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14271 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/release_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:10.834798 pulumi_lidarr-2.0.0a9/pulumi_lidarr/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/system/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/system/get_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17897 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/system/get_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26639 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/system/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23157 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/system/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:10.834798 pulumi_lidarr-2.0.0a9/pulumi_lidarr/tags/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/tags/get_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/tags/get_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/tags/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr/tags/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:29:10.806798 pulumi_lidarr-2.0.0a9/pulumi_lidarr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/pulumi_lidarr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:29:10.834798 pulumi_lidarr-2.0.0a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-25 16:29:10.000000 pulumi_lidarr-2.0.0a9/setup.py
```

### Comparing `pulumi_lidarr-2.0.0a8/PKG-INFO` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi_lidarr
-Version: 2.0.0a8
+Name: pulumi-lidarr
+Version: 2.0.0a9
 Summary: A Pulumi package for creating and managing Lidarr resources
 Home-page: https://github.com/MaienM/pulumi-lidarr
 License: Apache-2.0
 Project-URL: Repository, https://github.com/MaienM/pulumi-lidarr
 Keywords: pulumi lidarr category/utility
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_lidarr-2.0.0a8/README.md` & `pulumi_lidarr-2.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/__init__.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -445,14 +445,22 @@
   "fqn": "pulumi_lidarr.metadata",
   "classes": {
    "lidarr:Metadata/metadata:Metadata": "Metadata"
   }
  },
  {
   "pkg": "lidarr",
+  "mod": "Metadata/profile",
+  "fqn": "pulumi_lidarr.metadata",
+  "classes": {
+   "lidarr:Metadata/profile:Profile": "Profile"
+  }
+ },
+ {
+  "pkg": "lidarr",
   "mod": "Metadata/roksbox",
   "fqn": "pulumi_lidarr.metadata",
   "classes": {
    "lidarr:Metadata/roksbox:Roksbox": "Roksbox"
   }
  },
  {
@@ -669,42 +677,34 @@
   "fqn": "pulumi_lidarr.profiles",
   "classes": {
    "lidarr:Profiles/customFormat:CustomFormat": "CustomFormat"
   }
  },
  {
   "pkg": "lidarr",
-  "mod": "Profiles/delayProfile",
-  "fqn": "pulumi_lidarr.profiles",
-  "classes": {
-   "lidarr:Profiles/delayProfile:DelayProfile": "DelayProfile"
-  }
- },
- {
-  "pkg": "lidarr",
-  "mod": "Profiles/metadataProfile",
+  "mod": "Profiles/definition",
   "fqn": "pulumi_lidarr.profiles",
   "classes": {
-   "lidarr:Profiles/metadataProfile:MetadataProfile": "MetadataProfile"
+   "lidarr:Profiles/definition:Definition": "Definition"
   }
  },
  {
   "pkg": "lidarr",
-  "mod": "Profiles/qualityDefinition",
+  "mod": "Profiles/delayProfile",
   "fqn": "pulumi_lidarr.profiles",
   "classes": {
-   "lidarr:Profiles/qualityDefinition:QualityDefinition": "QualityDefinition"
+   "lidarr:Profiles/delayProfile:DelayProfile": "DelayProfile"
   }
  },
  {
   "pkg": "lidarr",
-  "mod": "Profiles/qualityProfile",
+  "mod": "Profiles/profile",
   "fqn": "pulumi_lidarr.profiles",
   "classes": {
-   "lidarr:Profiles/qualityProfile:QualityProfile": "QualityProfile"
+   "lidarr:Profiles/profile:Profile": "Profile"
   }
  },
  {
   "pkg": "lidarr",
   "mod": "Profiles/releaseProfile",
   "fqn": "pulumi_lidarr.profiles",
   "classes": {
```

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/_utilities.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/artists/artist.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/artists/artist.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/artists/get_artist.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/artists/get_artist.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/artists/get_artists.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/artists/get_artists.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/artists/outputs.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/artists/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/config/vars.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/__init__.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/aria2.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/aria2.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/config.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/config.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/deluge.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/deluge.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/download_client.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/download_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/flood.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/flood.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/get_config.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/get_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/get_download_client.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/get_download_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/get_download_clients.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/get_download_clients.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/get_remote_path_mapping.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/get_remote_path_mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/get_remote_path_mappings.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/get_remote_path_mappings.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/hadouken.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/hadouken.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/nzbget.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/nzbget.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/nzbvortex.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/nzbvortex.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/outputs.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/pneumatic.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/pneumatic.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/qbittorrent.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/qbittorrent.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/remote_path_mapping.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/remote_path_mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/rtorrent.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/rtorrent.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/sabnzbd.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/sabnzbd.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/torrent_blackhole.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/torrent_blackhole.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/torrent_download_station.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/torrent_download_station.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/transmission.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/transmission.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/usenet_blackhole.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/usenet_blackhole.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/usenet_download_station.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/usenet_download_station.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/utorrent.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/utorrent.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/downloadclients/vuze.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/downloadclients/vuze.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/__init__.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/exclusion.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/exclusion.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/get_exclusion.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/get_exclusion.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/get_exclusions.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/get_exclusions.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/get_import_list.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/get_import_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/get_import_lists.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/get_import_lists.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/headphones.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/headphones.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/import_list.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/import_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/lastfm_tag.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/lastfm_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/lastfm_user.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/lastfm_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/lidarr.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/lidarr.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/lidarr_list.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/lidarr_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/music_brainz.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/music_brainz.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/outputs.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/spotify_albums.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/spotify_albums.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/spotify_artists.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/spotify_artists.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/importlists/spotify_playlists.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/importlists/spotify_playlists.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/__init__.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/config.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/config.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/filelist.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/filelist.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/gazelle.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/gazelle.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/get_config.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/get_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/get_indexer.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/get_indexer.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/get_indexers.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/get_indexers.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/headphones.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/headphones.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/indexer.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/indexer.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/iptorrents.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/iptorrents.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/newznab.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/newznab.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/nyaa.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/nyaa.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/outputs.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/redacted.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/redacted.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/torrent_rss.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/torrent_rss.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/torrentleech.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/torrentleech.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/indexers/torznab.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/indexers/torznab.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/mediamanagement/get_media_management.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/mediamanagement/get_media_management.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/mediamanagement/get_naming.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/mediamanagement/get_naming.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/mediamanagement/get_root_folder.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/mediamanagement/get_root_folder.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/mediamanagement/get_root_folders.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/mediamanagement/get_root_folders.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/mediamanagement/media_management.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/mediamanagement/media_management.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/mediamanagement/naming.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/mediamanagement/naming.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/mediamanagement/outputs.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/mediamanagement/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/mediamanagement/root_folder.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/mediamanagement/root_folder.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/metadata/config.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/metadata/config.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/metadata/get_config.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/metadata/get_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/metadata/get_consumers.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/metadata/get_consumers.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/metadata/get_metadata.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/metadata/get_metadata.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/metadata/kodi.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/metadata/kodi.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/metadata/metadata.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/metadata/roksbox.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/metadata/roksbox.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/metadata/wdtv.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/metadata/wdtv.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/__init__.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/apprise.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/apprise.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/custom_script.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/custom_script.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/discord.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/discord.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/email.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/email.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/emby.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/emby.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/get_notification.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/get_notification.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/get_notifications.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/get_notifications.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/gotify.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/gotify.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/join.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/join.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/kodi.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/kodi.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/mailgun.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/mailgun.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/notifiarr.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/notifiarr.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/notification.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/notification.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/ntfy.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/ntfy.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/outputs.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/plex.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/plex.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/prowl.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/prowl.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/pushbullet.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/pushbullet.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/pushover.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/pushover.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/sendgrid.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/sendgrid.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/signal.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/signal.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/simplepush.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/simplepush.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/slack.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/slack.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/subsonic.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/subsonic.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/synology_indexer.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/synology_indexer.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/telegram.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/telegram.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/twitter.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/twitter.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/notifications/webhook.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/notifications/webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/__init__.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,37 +2,34 @@
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from .. import _utilities
 import typing
 # Export this package's modules as members:
 from .custom_format import *
+from .definition import *
 from .delay_profile import *
 from .get_condition import *
 from .get_condition_release_group import *
 from .get_condition_release_title import *
 from .get_condition_size import *
 from .get_custom_format import *
 from .get_custom_formats import *
+from .get_definition import *
+from .get_definitions import *
 from .get_delay_profile import *
 from .get_delay_profiles import *
-from .get_metadata_profile import *
-from .get_metadata_profiles import *
 from .get_primary_album_type import *
 from .get_primary_album_types import *
+from .get_profile import *
+from .get_profiles import *
 from .get_quality import *
-from .get_quality_definition import *
-from .get_quality_definitions import *
-from .get_quality_profile import *
-from .get_quality_profiles import *
 from .get_release_profile import *
 from .get_release_profiles import *
 from .get_release_status import *
 from .get_release_statuses import *
 from .get_secondary_album_type import *
 from .get_secondary_album_types import *
-from .metadata_profile import *
-from .quality_definition import *
-from .quality_profile import *
+from .profile import *
 from .release_profile import *
 from ._inputs import *
 from . import outputs
```

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/_inputs.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
     'CustomFormatSpecificationArgs',
-    'QualityProfileFormatItemArgs',
-    'QualityProfileQualityGroupArgs',
-    'QualityProfileQualityGroupQualityArgs',
+    'ProfileFormatItemArgs',
+    'ProfileQualityGroupArgs',
+    'ProfileQualityGroupQualityArgs',
 ]
 
 @pulumi.input_type
 class CustomFormatSpecificationArgs:
     def __init__(__self__, *,
                  implementation: Optional[pulumi.Input[str]] = None,
                  max: Optional[pulumi.Input[int]] = None,
@@ -132,15 +132,15 @@
 
     @value.setter
     def value(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "value", value)
 
 
 @pulumi.input_type
-class QualityProfileFormatItemArgs:
+class ProfileFormatItemArgs:
     def __init__(__self__, *,
                  format: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  score: Optional[pulumi.Input[int]] = None):
         """
         :param pulumi.Input[int] format: Format.
         :param pulumi.Input[str] name: Name.
@@ -187,40 +187,40 @@
 
     @score.setter
     def score(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "score", value)
 
 
 @pulumi.input_type
-class QualityProfileQualityGroupArgs:
+class ProfileQualityGroupArgs:
     def __init__(__self__, *,
-                 qualities: pulumi.Input[Sequence[pulumi.Input['QualityProfileQualityGroupQualityArgs']]],
+                 qualities: pulumi.Input[Sequence[pulumi.Input['ProfileQualityGroupQualityArgs']]],
                  id: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[Sequence[pulumi.Input['QualityProfileQualityGroupQualityArgs']]] qualities: Ordered list of qualities in group.
+        :param pulumi.Input[Sequence[pulumi.Input['ProfileQualityGroupQualityArgs']]] qualities: Ordered list of qualities in group.
         :param pulumi.Input[int] id: Quality group ID.
         :param pulumi.Input[str] name: Quality group name.
         """
         pulumi.set(__self__, "qualities", qualities)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
-    def qualities(self) -> pulumi.Input[Sequence[pulumi.Input['QualityProfileQualityGroupQualityArgs']]]:
+    def qualities(self) -> pulumi.Input[Sequence[pulumi.Input['ProfileQualityGroupQualityArgs']]]:
         """
         Ordered list of qualities in group.
         """
         return pulumi.get(self, "qualities")
 
     @qualities.setter
-    def qualities(self, value: pulumi.Input[Sequence[pulumi.Input['QualityProfileQualityGroupQualityArgs']]]):
+    def qualities(self, value: pulumi.Input[Sequence[pulumi.Input['ProfileQualityGroupQualityArgs']]]):
         pulumi.set(self, "qualities", value)
 
     @property
     @pulumi.getter
     def id(self) -> Optional[pulumi.Input[int]]:
         """
         Quality group ID.
@@ -241,15 +241,15 @@
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
 
 @pulumi.input_type
-class QualityProfileQualityGroupQualityArgs:
+class ProfileQualityGroupQualityArgs:
     def __init__(__self__, *,
                  id: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[int] id: Quality group ID.
         :param pulumi.Input[str] name: Name.
         """
```

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/custom_format.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/custom_format.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/delay_profile.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/delay_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_condition.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_condition.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_condition_release_group.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_condition_release_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_condition_release_title.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_condition_release_title.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_condition_size.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_condition_size.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_custom_format.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_custom_format.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_custom_formats.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_custom_formats.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_delay_profile.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_delay_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_delay_profiles.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_delay_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_metadata_profile.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/metadata/get_profile.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
-    'GetMetadataProfileResult',
-    'AwaitableGetMetadataProfileResult',
-    'get_metadata_profile',
-    'get_metadata_profile_output',
+    'GetProfileResult',
+    'AwaitableGetProfileResult',
+    'get_profile',
+    'get_profile_output',
 ]
 
 @pulumi.output_type
-class GetMetadataProfileResult:
+class GetProfileResult:
     """
-    A collection of values returned by getMetadataProfile.
+    A collection of values returned by getProfile.
     """
     def __init__(__self__, id=None, name=None, primary_album_types=None, release_statuses=None, secondary_album_types=None):
         if id and not isinstance(id, int):
             raise TypeError("Expected argument 'id' to be a int")
         pulumi.set(__self__, "id", id)
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
@@ -75,69 +75,69 @@
     def secondary_album_types(self) -> Sequence[int]:
         """
         Secondary album types.
         """
         return pulumi.get(self, "secondary_album_types")
 
 
-class AwaitableGetMetadataProfileResult(GetMetadataProfileResult):
+class AwaitableGetProfileResult(GetProfileResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetMetadataProfileResult(
+        return GetProfileResult(
             id=self.id,
             name=self.name,
             primary_album_types=self.primary_album_types,
             release_statuses=self.release_statuses,
             secondary_album_types=self.secondary_album_types)
 
 
-def get_metadata_profile(name: Optional[str] = None,
-                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetMetadataProfileResult:
+def get_profile(name: Optional[str] = None,
+                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetProfileResult:
     """
     <!-- subcategory:Profiles -->Single Metadata Profile.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_lidarr as lidarr
 
-    example = lidarr.Profiles.get_metadata_profile(name="Example")
+    example = lidarr.Metadata.get_profile(name="Example")
     ```
 
 
     :param str name: Metadata Profile name.
     """
     __args__ = dict()
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('lidarr:Profiles/getMetadataProfile:getMetadataProfile', __args__, opts=opts, typ=GetMetadataProfileResult).value
+    __ret__ = pulumi.runtime.invoke('lidarr:Metadata/getProfile:getProfile', __args__, opts=opts, typ=GetProfileResult).value
 
-    return AwaitableGetMetadataProfileResult(
+    return AwaitableGetProfileResult(
         id=pulumi.get(__ret__, 'id'),
         name=pulumi.get(__ret__, 'name'),
         primary_album_types=pulumi.get(__ret__, 'primary_album_types'),
         release_statuses=pulumi.get(__ret__, 'release_statuses'),
         secondary_album_types=pulumi.get(__ret__, 'secondary_album_types'))
 
 
-@_utilities.lift_output_func(get_metadata_profile)
-def get_metadata_profile_output(name: Optional[pulumi.Input[str]] = None,
-                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetMetadataProfileResult]:
+@_utilities.lift_output_func(get_profile)
+def get_profile_output(name: Optional[pulumi.Input[str]] = None,
+                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProfileResult]:
     """
     <!-- subcategory:Profiles -->Single Metadata Profile.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_lidarr as lidarr
 
-    example = lidarr.Profiles.get_metadata_profile(name="Example")
+    example = lidarr.Metadata.get_profile(name="Example")
     ```
 
 
     :param str name: Metadata Profile name.
     """
     ...
```

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_metadata_profiles.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_release_profiles.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,90 +7,90 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 
 __all__ = [
-    'GetMetadataProfilesResult',
-    'AwaitableGetMetadataProfilesResult',
-    'get_metadata_profiles',
-    'get_metadata_profiles_output',
+    'GetReleaseProfilesResult',
+    'AwaitableGetReleaseProfilesResult',
+    'get_release_profiles',
+    'get_release_profiles_output',
 ]
 
 @pulumi.output_type
-class GetMetadataProfilesResult:
+class GetReleaseProfilesResult:
     """
-    A collection of values returned by getMetadataProfiles.
+    A collection of values returned by getReleaseProfiles.
     """
-    def __init__(__self__, id=None, metadata_profiles=None):
+    def __init__(__self__, id=None, release_profiles=None):
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if metadata_profiles and not isinstance(metadata_profiles, list):
-            raise TypeError("Expected argument 'metadata_profiles' to be a list")
-        pulumi.set(__self__, "metadata_profiles", metadata_profiles)
+        if release_profiles and not isinstance(release_profiles, list):
+            raise TypeError("Expected argument 'release_profiles' to be a list")
+        pulumi.set(__self__, "release_profiles", release_profiles)
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The ID of this resource.
         """
         return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter(name="metadataProfiles")
-    def metadata_profiles(self) -> Sequence['outputs.GetMetadataProfilesMetadataProfileResult']:
+    @pulumi.getter(name="releaseProfiles")
+    def release_profiles(self) -> Sequence['outputs.GetReleaseProfilesReleaseProfileResult']:
         """
-        Metadata Profile list.
+        Release Profile list.
         """
-        return pulumi.get(self, "metadata_profiles")
+        return pulumi.get(self, "release_profiles")
 
 
-class AwaitableGetMetadataProfilesResult(GetMetadataProfilesResult):
+class AwaitableGetReleaseProfilesResult(GetReleaseProfilesResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetMetadataProfilesResult(
+        return GetReleaseProfilesResult(
             id=self.id,
-            metadata_profiles=self.metadata_profiles)
+            release_profiles=self.release_profiles)
 
 
-def get_metadata_profiles(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetMetadataProfilesResult:
+def get_release_profiles(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetReleaseProfilesResult:
     """
-    <!-- subcategory:Profiles -->List all available Metadata Profiles.
+    <!-- subcategory:Profiles -->List all available Release Profiles.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_lidarr as lidarr
 
-    example = lidarr.Profiles.get_metadata_profiles()
+    example = lidarr.Profiles.get_release_profiles()
     ```
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('lidarr:Profiles/getMetadataProfiles:getMetadataProfiles', __args__, opts=opts, typ=GetMetadataProfilesResult).value
+    __ret__ = pulumi.runtime.invoke('lidarr:Profiles/getReleaseProfiles:getReleaseProfiles', __args__, opts=opts, typ=GetReleaseProfilesResult).value
 
-    return AwaitableGetMetadataProfilesResult(
+    return AwaitableGetReleaseProfilesResult(
         id=pulumi.get(__ret__, 'id'),
-        metadata_profiles=pulumi.get(__ret__, 'metadata_profiles'))
+        release_profiles=pulumi.get(__ret__, 'release_profiles'))
 
 
-@_utilities.lift_output_func(get_metadata_profiles)
-def get_metadata_profiles_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetMetadataProfilesResult]:
+@_utilities.lift_output_func(get_release_profiles)
+def get_release_profiles_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetReleaseProfilesResult]:
     """
-    <!-- subcategory:Profiles -->List all available Metadata Profiles.
+    <!-- subcategory:Profiles -->List all available Release Profiles.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_lidarr as lidarr
 
-    example = lidarr.Profiles.get_metadata_profiles()
+    example = lidarr.Profiles.get_release_profiles()
     ```
     """
     ...
```

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_primary_album_type.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_primary_album_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_primary_album_types.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_primary_album_types.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_quality.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_quality.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_quality_definition.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_definition.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
-    'GetQualityDefinitionResult',
-    'AwaitableGetQualityDefinitionResult',
-    'get_quality_definition',
-    'get_quality_definition_output',
+    'GetDefinitionResult',
+    'AwaitableGetDefinitionResult',
+    'get_definition',
+    'get_definition_output',
 ]
 
 @pulumi.output_type
-class GetQualityDefinitionResult:
+class GetDefinitionResult:
     """
-    A collection of values returned by getQualityDefinition.
+    A collection of values returned by getDefinition.
     """
     def __init__(__self__, id=None, max_size=None, min_size=None, quality_id=None, quality_name=None, title=None):
         if id and not isinstance(id, int):
             raise TypeError("Expected argument 'id' to be a int")
         pulumi.set(__self__, "id", id)
         if max_size and not isinstance(max_size, float):
             raise TypeError("Expected argument 'max_size' to be a float")
@@ -86,76 +86,76 @@
     def title(self) -> str:
         """
         Quality Definition Title.
         """
         return pulumi.get(self, "title")
 
 
-class AwaitableGetQualityDefinitionResult(GetQualityDefinitionResult):
+class AwaitableGetDefinitionResult(GetDefinitionResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetQualityDefinitionResult(
+        return GetDefinitionResult(
             id=self.id,
             max_size=self.max_size,
             min_size=self.min_size,
             quality_id=self.quality_id,
             quality_name=self.quality_name,
             title=self.title)
 
 
-def get_quality_definition(id: Optional[int] = None,
-                           min_size: Optional[float] = None,
-                           opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetQualityDefinitionResult:
+def get_definition(id: Optional[int] = None,
+                   min_size: Optional[float] = None,
+                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDefinitionResult:
     """
     <!-- subcategory:Profiles -->Single Quality Definition.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_lidarr as lidarr
 
-    example = lidarr.Profiles.get_quality_definition(id=32)
+    example = lidarr.Profiles.get_definition(id=32)
     ```
 
 
     :param int id: Quality Definition ID.
     :param float min_size: Minimum size MB/min.
     """
     __args__ = dict()
     __args__['id'] = id
     __args__['minSize'] = min_size
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('lidarr:Profiles/getQualityDefinition:getQualityDefinition', __args__, opts=opts, typ=GetQualityDefinitionResult).value
+    __ret__ = pulumi.runtime.invoke('lidarr:Profiles/getDefinition:getDefinition', __args__, opts=opts, typ=GetDefinitionResult).value
 
-    return AwaitableGetQualityDefinitionResult(
+    return AwaitableGetDefinitionResult(
         id=pulumi.get(__ret__, 'id'),
         max_size=pulumi.get(__ret__, 'max_size'),
         min_size=pulumi.get(__ret__, 'min_size'),
         quality_id=pulumi.get(__ret__, 'quality_id'),
         quality_name=pulumi.get(__ret__, 'quality_name'),
         title=pulumi.get(__ret__, 'title'))
 
 
-@_utilities.lift_output_func(get_quality_definition)
-def get_quality_definition_output(id: Optional[pulumi.Input[int]] = None,
-                                  min_size: Optional[pulumi.Input[Optional[float]]] = None,
-                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetQualityDefinitionResult]:
+@_utilities.lift_output_func(get_definition)
+def get_definition_output(id: Optional[pulumi.Input[int]] = None,
+                          min_size: Optional[pulumi.Input[Optional[float]]] = None,
+                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDefinitionResult]:
     """
     <!-- subcategory:Profiles -->Single Quality Definition.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_lidarr as lidarr
 
-    example = lidarr.Profiles.get_quality_definition(id=32)
+    example = lidarr.Profiles.get_definition(id=32)
     ```
 
 
     :param int id: Quality Definition ID.
     :param float min_size: Minimum size MB/min.
     """
     ...
```

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_quality_definitions.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_definitions.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 
 __all__ = [
-    'GetQualityDefinitionsResult',
-    'AwaitableGetQualityDefinitionsResult',
-    'get_quality_definitions',
-    'get_quality_definitions_output',
+    'GetDefinitionsResult',
+    'AwaitableGetDefinitionsResult',
+    'get_definitions',
+    'get_definitions_output',
 ]
 
 @pulumi.output_type
-class GetQualityDefinitionsResult:
+class GetDefinitionsResult:
     """
-    A collection of values returned by getQualityDefinitions.
+    A collection of values returned by getDefinitions.
     """
     def __init__(__self__, id=None, quality_definitions=None):
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if quality_definitions and not isinstance(quality_definitions, list):
             raise TypeError("Expected argument 'quality_definitions' to be a list")
@@ -36,61 +36,61 @@
         """
         The ID of this resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="qualityDefinitions")
-    def quality_definitions(self) -> Sequence['outputs.GetQualityDefinitionsQualityDefinitionResult']:
+    def quality_definitions(self) -> Sequence['outputs.GetDefinitionsQualityDefinitionResult']:
         """
         Quality Definition list.
         """
         return pulumi.get(self, "quality_definitions")
 
 
-class AwaitableGetQualityDefinitionsResult(GetQualityDefinitionsResult):
+class AwaitableGetDefinitionsResult(GetDefinitionsResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetQualityDefinitionsResult(
+        return GetDefinitionsResult(
             id=self.id,
             quality_definitions=self.quality_definitions)
 
 
-def get_quality_definitions(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetQualityDefinitionsResult:
+def get_definitions(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDefinitionsResult:
     """
     <!-- subcategory:Profiles -->List all available Quality Definitions.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_lidarr as lidarr
 
-    example = lidarr.Profiles.get_quality_definitions()
+    example = lidarr.Profiles.get_definitions()
     ```
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('lidarr:Profiles/getQualityDefinitions:getQualityDefinitions', __args__, opts=opts, typ=GetQualityDefinitionsResult).value
+    __ret__ = pulumi.runtime.invoke('lidarr:Profiles/getDefinitions:getDefinitions', __args__, opts=opts, typ=GetDefinitionsResult).value
 
-    return AwaitableGetQualityDefinitionsResult(
+    return AwaitableGetDefinitionsResult(
         id=pulumi.get(__ret__, 'id'),
         quality_definitions=pulumi.get(__ret__, 'quality_definitions'))
 
 
-@_utilities.lift_output_func(get_quality_definitions)
-def get_quality_definitions_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetQualityDefinitionsResult]:
+@_utilities.lift_output_func(get_definitions)
+def get_definitions_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDefinitionsResult]:
     """
     <!-- subcategory:Profiles -->List all available Quality Definitions.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_lidarr as lidarr
 
-    example = lidarr.Profiles.get_quality_definitions()
+    example = lidarr.Profiles.get_definitions()
     ```
     """
     ...
```

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_quality_profile.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_profile.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 
 __all__ = [
-    'GetQualityProfileResult',
-    'AwaitableGetQualityProfileResult',
-    'get_quality_profile',
-    'get_quality_profile_output',
+    'GetProfileResult',
+    'AwaitableGetProfileResult',
+    'get_profile',
+    'get_profile_output',
 ]
 
 @pulumi.output_type
-class GetQualityProfileResult:
+class GetProfileResult:
     """
-    A collection of values returned by getQualityProfile.
+    A collection of values returned by getProfile.
     """
     def __init__(__self__, cutoff=None, cutoff_format_score=None, format_items=None, id=None, min_format_score=None, name=None, quality_groups=None, upgrade_allowed=None):
         if cutoff and not isinstance(cutoff, int):
             raise TypeError("Expected argument 'cutoff' to be a int")
         pulumi.set(__self__, "cutoff", cutoff)
         if cutoff_format_score and not isinstance(cutoff_format_score, int):
             raise TypeError("Expected argument 'cutoff_format_score' to be a int")
@@ -62,15 +62,15 @@
         """
         Cutoff format score.
         """
         return pulumi.get(self, "cutoff_format_score")
 
     @property
     @pulumi.getter(name="formatItems")
-    def format_items(self) -> Sequence['outputs.GetQualityProfileFormatItemResult']:
+    def format_items(self) -> Sequence['outputs.GetProfileFormatItemResult']:
         """
         Format items.
         """
         return pulumi.get(self, "format_items")
 
     @property
     @pulumi.getter
@@ -94,90 +94,90 @@
         """
         Quality Profile Name.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="qualityGroups")
-    def quality_groups(self) -> Sequence['outputs.GetQualityProfileQualityGroupResult']:
+    def quality_groups(self) -> Sequence['outputs.GetProfileQualityGroupResult']:
         """
         Quality groups.
         """
         return pulumi.get(self, "quality_groups")
 
     @property
     @pulumi.getter(name="upgradeAllowed")
     def upgrade_allowed(self) -> bool:
         """
         Upgrade allowed flag.
         """
         return pulumi.get(self, "upgrade_allowed")
 
 
-class AwaitableGetQualityProfileResult(GetQualityProfileResult):
+class AwaitableGetProfileResult(GetProfileResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetQualityProfileResult(
+        return GetProfileResult(
             cutoff=self.cutoff,
             cutoff_format_score=self.cutoff_format_score,
             format_items=self.format_items,
             id=self.id,
             min_format_score=self.min_format_score,
             name=self.name,
             quality_groups=self.quality_groups,
             upgrade_allowed=self.upgrade_allowed)
 
 
-def get_quality_profile(name: Optional[str] = None,
-                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetQualityProfileResult:
+def get_profile(name: Optional[str] = None,
+                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetProfileResult:
     """
     <!-- subcategory:Profiles -->Single Quality Profile.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_lidarr as lidarr
 
-    example = lidarr.Profiles.get_quality_profile(name="Example")
+    example = lidarr.Profiles.get_profile(name="Example")
     ```
 
 
     :param str name: Name.
     """
     __args__ = dict()
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('lidarr:Profiles/getQualityProfile:getQualityProfile', __args__, opts=opts, typ=GetQualityProfileResult).value
+    __ret__ = pulumi.runtime.invoke('lidarr:Profiles/getProfile:getProfile', __args__, opts=opts, typ=GetProfileResult).value
 
-    return AwaitableGetQualityProfileResult(
+    return AwaitableGetProfileResult(
         cutoff=pulumi.get(__ret__, 'cutoff'),
         cutoff_format_score=pulumi.get(__ret__, 'cutoff_format_score'),
         format_items=pulumi.get(__ret__, 'format_items'),
         id=pulumi.get(__ret__, 'id'),
         min_format_score=pulumi.get(__ret__, 'min_format_score'),
         name=pulumi.get(__ret__, 'name'),
         quality_groups=pulumi.get(__ret__, 'quality_groups'),
         upgrade_allowed=pulumi.get(__ret__, 'upgrade_allowed'))
 
 
-@_utilities.lift_output_func(get_quality_profile)
-def get_quality_profile_output(name: Optional[pulumi.Input[str]] = None,
-                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetQualityProfileResult]:
+@_utilities.lift_output_func(get_profile)
+def get_profile_output(name: Optional[pulumi.Input[str]] = None,
+                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProfileResult]:
     """
     <!-- subcategory:Profiles -->Single Quality Profile.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_lidarr as lidarr
 
-    example = lidarr.Profiles.get_quality_profile(name="Example")
+    example = lidarr.Profiles.get_profile(name="Example")
     ```
 
 
     :param str name: Name.
     """
     ...
```

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_quality_profiles.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_profiles.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 
 __all__ = [
-    'GetQualityProfilesResult',
-    'AwaitableGetQualityProfilesResult',
-    'get_quality_profiles',
-    'get_quality_profiles_output',
+    'GetProfilesResult',
+    'AwaitableGetProfilesResult',
+    'get_profiles',
+    'get_profiles_output',
 ]
 
 @pulumi.output_type
-class GetQualityProfilesResult:
+class GetProfilesResult:
     """
-    A collection of values returned by getQualityProfiles.
+    A collection of values returned by getProfiles.
     """
     def __init__(__self__, id=None, quality_profiles=None):
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if quality_profiles and not isinstance(quality_profiles, list):
             raise TypeError("Expected argument 'quality_profiles' to be a list")
@@ -36,61 +36,61 @@
         """
         The ID of this resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="qualityProfiles")
-    def quality_profiles(self) -> Sequence['outputs.GetQualityProfilesQualityProfileResult']:
+    def quality_profiles(self) -> Sequence['outputs.GetProfilesQualityProfileResult']:
         """
         Quality Profile list.
         """
         return pulumi.get(self, "quality_profiles")
 
 
-class AwaitableGetQualityProfilesResult(GetQualityProfilesResult):
+class AwaitableGetProfilesResult(GetProfilesResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetQualityProfilesResult(
+        return GetProfilesResult(
             id=self.id,
             quality_profiles=self.quality_profiles)
 
 
-def get_quality_profiles(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetQualityProfilesResult:
+def get_profiles(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetProfilesResult:
     """
     <!-- subcategory:Profiles -->List all available Quality Profiles.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_lidarr as lidarr
 
-    example = lidarr.Profiles.get_quality_profiles()
+    example = lidarr.Profiles.get_profiles()
     ```
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('lidarr:Profiles/getQualityProfiles:getQualityProfiles', __args__, opts=opts, typ=GetQualityProfilesResult).value
+    __ret__ = pulumi.runtime.invoke('lidarr:Profiles/getProfiles:getProfiles', __args__, opts=opts, typ=GetProfilesResult).value
 
-    return AwaitableGetQualityProfilesResult(
+    return AwaitableGetProfilesResult(
         id=pulumi.get(__ret__, 'id'),
         quality_profiles=pulumi.get(__ret__, 'quality_profiles'))
 
 
-@_utilities.lift_output_func(get_quality_profiles)
-def get_quality_profiles_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetQualityProfilesResult]:
+@_utilities.lift_output_func(get_profiles)
+def get_profiles_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProfilesResult]:
     """
     <!-- subcategory:Profiles -->List all available Quality Profiles.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_lidarr as lidarr
 
-    example = lidarr.Profiles.get_quality_profiles()
+    example = lidarr.Profiles.get_profiles()
     ```
     """
     ...
```

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_release_profile.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_release_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_release_status.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_release_status.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_release_statuses.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_release_statuses.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_secondary_album_type.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_secondary_album_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/get_secondary_album_types.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/get_secondary_album_types.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/metadata_profile.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/metadata/profile.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
-__all__ = ['MetadataProfileArgs', 'MetadataProfile']
+__all__ = ['ProfileArgs', 'Profile']
 
 @pulumi.input_type
-class MetadataProfileArgs:
+class ProfileArgs:
     def __init__(__self__, *,
                  primary_album_types: pulumi.Input[Sequence[pulumi.Input[int]]],
                  release_statuses: pulumi.Input[Sequence[pulumi.Input[int]]],
                  secondary_album_types: pulumi.Input[Sequence[pulumi.Input[int]]],
                  name: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a MetadataProfile resource.
+        The set of arguments for constructing a Profile resource.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] primary_album_types: Primary album types.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] release_statuses: Release statuses.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] secondary_album_types: Secondary album types.
         :param pulumi.Input[str] name: Metadata Profile name.
         """
         pulumi.set(__self__, "primary_album_types", primary_album_types)
         pulumi.set(__self__, "release_statuses", release_statuses)
@@ -77,22 +77,22 @@
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
 
 @pulumi.input_type
-class _MetadataProfileState:
+class _ProfileState:
     def __init__(__self__, *,
                  name: Optional[pulumi.Input[str]] = None,
                  primary_album_types: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
                  release_statuses: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
                  secondary_album_types: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None):
         """
-        Input properties used for looking up and filtering MetadataProfile resources.
+        Input properties used for looking up and filtering Profile resources.
         :param pulumi.Input[str] name: Metadata Profile name.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] primary_album_types: Primary album types.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] release_statuses: Release statuses.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] secondary_album_types: Secondary album types.
         """
         if name is not None:
             pulumi.set(__self__, "name", name)
@@ -148,15 +148,15 @@
         return pulumi.get(self, "secondary_album_types")
 
     @secondary_album_types.setter
     def secondary_album_types(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]]):
         pulumi.set(self, "secondary_album_types", value)
 
 
-class MetadataProfile(pulumi.CustomResource):
+class Profile(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  primary_album_types: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
                  release_statuses: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
@@ -168,78 +168,78 @@
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_lidarr as lidarr
 
-        example = lidarr.profiles.MetadataProfile("example",
+        example = lidarr.metadata.Profile("example",
             primary_album_types=[
                 1,
                 2,
             ],
             release_statuses=[3],
             secondary_album_types=[1])
         ```
 
         ## Import
 
         import using the API/UI ID
 
         ```sh
-         $ pulumi import lidarr:Profiles/metadataProfile:MetadataProfile example 10
+         $ pulumi import lidarr:Metadata/profile:Profile example 10
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: Metadata Profile name.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] primary_album_types: Primary album types.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] release_statuses: Release statuses.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] secondary_album_types: Secondary album types.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: MetadataProfileArgs,
+                 args: ProfileArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         <!-- subcategory:Profiles -->Metadata Profile resource.
         For more information refer to [Metadata Profile](https://wiki.servarr.com/lidarr/settings#metadata-profiles) documentation.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_lidarr as lidarr
 
-        example = lidarr.profiles.MetadataProfile("example",
+        example = lidarr.metadata.Profile("example",
             primary_album_types=[
                 1,
                 2,
             ],
             release_statuses=[3],
             secondary_album_types=[1])
         ```
 
         ## Import
 
         import using the API/UI ID
 
         ```sh
-         $ pulumi import lidarr:Profiles/metadataProfile:MetadataProfile example 10
+         $ pulumi import lidarr:Metadata/profile:Profile example 10
         ```
 
         :param str resource_name: The name of the resource.
-        :param MetadataProfileArgs args: The arguments to use to populate this resource's properties.
+        :param ProfileArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(MetadataProfileArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(ProfileArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -251,61 +251,61 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = MetadataProfileArgs.__new__(MetadataProfileArgs)
+            __props__ = ProfileArgs.__new__(ProfileArgs)
 
             __props__.__dict__["name"] = name
             if primary_album_types is None and not opts.urn:
                 raise TypeError("Missing required property 'primary_album_types'")
             __props__.__dict__["primary_album_types"] = primary_album_types
             if release_statuses is None and not opts.urn:
                 raise TypeError("Missing required property 'release_statuses'")
             __props__.__dict__["release_statuses"] = release_statuses
             if secondary_album_types is None and not opts.urn:
                 raise TypeError("Missing required property 'secondary_album_types'")
             __props__.__dict__["secondary_album_types"] = secondary_album_types
-        super(MetadataProfile, __self__).__init__(
-            'lidarr:Profiles/metadataProfile:MetadataProfile',
+        super(Profile, __self__).__init__(
+            'lidarr:Metadata/profile:Profile',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             name: Optional[pulumi.Input[str]] = None,
             primary_album_types: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
             release_statuses: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
-            secondary_album_types: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None) -> 'MetadataProfile':
+            secondary_album_types: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None) -> 'Profile':
         """
-        Get an existing MetadataProfile resource's state with the given name, id, and optional extra
+        Get an existing Profile resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: Metadata Profile name.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] primary_album_types: Primary album types.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] release_statuses: Release statuses.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] secondary_album_types: Secondary album types.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _MetadataProfileState.__new__(_MetadataProfileState)
+        __props__ = _ProfileState.__new__(_ProfileState)
 
         __props__.__dict__["name"] = name
         __props__.__dict__["primary_album_types"] = primary_album_types
         __props__.__dict__["release_statuses"] = release_statuses
         __props__.__dict__["secondary_album_types"] = secondary_album_types
-        return MetadataProfile(resource_name, opts=opts, __props__=__props__)
+        return Profile(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
         Metadata Profile name.
         """
```

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/outputs.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,31 +8,30 @@
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 
 __all__ = [
     'CustomFormatSpecification',
-    'QualityProfileFormatItem',
-    'QualityProfileQualityGroup',
-    'QualityProfileQualityGroupQuality',
+    'ProfileFormatItem',
+    'ProfileQualityGroup',
+    'ProfileQualityGroupQuality',
     'GetCustomFormatSpecificationResult',
     'GetCustomFormatsCustomFormatResult',
     'GetCustomFormatsCustomFormatSpecificationResult',
+    'GetDefinitionsQualityDefinitionResult',
     'GetDelayProfilesDelayProfileResult',
-    'GetMetadataProfilesMetadataProfileResult',
     'GetPrimaryAlbumTypesElementResult',
-    'GetQualityDefinitionsQualityDefinitionResult',
-    'GetQualityProfileFormatItemResult',
-    'GetQualityProfileQualityGroupResult',
-    'GetQualityProfileQualityGroupQualityResult',
-    'GetQualityProfilesQualityProfileResult',
-    'GetQualityProfilesQualityProfileFormatItemResult',
-    'GetQualityProfilesQualityProfileQualityGroupResult',
-    'GetQualityProfilesQualityProfileQualityGroupQualityResult',
+    'GetProfileFormatItemResult',
+    'GetProfileQualityGroupResult',
+    'GetProfileQualityGroupQualityResult',
+    'GetProfilesQualityProfileResult',
+    'GetProfilesQualityProfileFormatItemResult',
+    'GetProfilesQualityProfileQualityGroupResult',
+    'GetProfilesQualityProfileQualityGroupQualityResult',
     'GetReleaseProfilesReleaseProfileResult',
     'GetReleaseStatusesElementResult',
     'GetSecondaryAlbumTypesElementResult',
 ]
 
 @pulumi.output_type
 class CustomFormatSpecification(dict):
@@ -122,15 +121,15 @@
         """
         Value.
         """
         return pulumi.get(self, "value")
 
 
 @pulumi.output_type
-class QualityProfileFormatItem(dict):
+class ProfileFormatItem(dict):
     def __init__(__self__, *,
                  format: Optional[int] = None,
                  name: Optional[str] = None,
                  score: Optional[int] = None):
         """
         :param int format: Format.
         :param str name: Name.
@@ -165,33 +164,33 @@
         """
         Score.
         """
         return pulumi.get(self, "score")
 
 
 @pulumi.output_type
-class QualityProfileQualityGroup(dict):
+class ProfileQualityGroup(dict):
     def __init__(__self__, *,
-                 qualities: Sequence['outputs.QualityProfileQualityGroupQuality'],
+                 qualities: Sequence['outputs.ProfileQualityGroupQuality'],
                  id: Optional[int] = None,
                  name: Optional[str] = None):
         """
-        :param Sequence['QualityProfileQualityGroupQualityArgs'] qualities: Ordered list of qualities in group.
+        :param Sequence['ProfileQualityGroupQualityArgs'] qualities: Ordered list of qualities in group.
         :param int id: Quality group ID.
         :param str name: Quality group name.
         """
         pulumi.set(__self__, "qualities", qualities)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
-    def qualities(self) -> Sequence['outputs.QualityProfileQualityGroupQuality']:
+    def qualities(self) -> Sequence['outputs.ProfileQualityGroupQuality']:
         """
         Ordered list of qualities in group.
         """
         return pulumi.get(self, "qualities")
 
     @property
     @pulumi.getter
@@ -207,15 +206,15 @@
         """
         Quality group name.
         """
         return pulumi.get(self, "name")
 
 
 @pulumi.output_type
-class QualityProfileQualityGroupQuality(dict):
+class ProfileQualityGroupQuality(dict):
     def __init__(__self__, *,
                  id: Optional[int] = None,
                  name: Optional[str] = None):
         """
         :param int id: Quality group ID.
         :param str name: Name.
         """
@@ -457,14 +456,87 @@
         """
         Value.
         """
         return pulumi.get(self, "value")
 
 
 @pulumi.output_type
+class GetDefinitionsQualityDefinitionResult(dict):
+    def __init__(__self__, *,
+                 id: int,
+                 max_size: float,
+                 min_size: float,
+                 quality_id: int,
+                 quality_name: str,
+                 title: str):
+        """
+        :param int id: Quality Definition ID.
+        :param float max_size: Maximum size MB/min.
+        :param float min_size: Minimum size MB/min.
+        :param int quality_id: Quality ID.
+        :param str quality_name: Quality Name.
+        :param str title: Quality Definition Title.
+        """
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "max_size", max_size)
+        pulumi.set(__self__, "min_size", min_size)
+        pulumi.set(__self__, "quality_id", quality_id)
+        pulumi.set(__self__, "quality_name", quality_name)
+        pulumi.set(__self__, "title", title)
+
+    @property
+    @pulumi.getter
+    def id(self) -> int:
+        """
+        Quality Definition ID.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter(name="maxSize")
+    def max_size(self) -> float:
+        """
+        Maximum size MB/min.
+        """
+        return pulumi.get(self, "max_size")
+
+    @property
+    @pulumi.getter(name="minSize")
+    def min_size(self) -> float:
+        """
+        Minimum size MB/min.
+        """
+        return pulumi.get(self, "min_size")
+
+    @property
+    @pulumi.getter(name="qualityId")
+    def quality_id(self) -> int:
+        """
+        Quality ID.
+        """
+        return pulumi.get(self, "quality_id")
+
+    @property
+    @pulumi.getter(name="qualityName")
+    def quality_name(self) -> str:
+        """
+        Quality Name.
+        """
+        return pulumi.get(self, "quality_name")
+
+    @property
+    @pulumi.getter
+    def title(self) -> str:
+        """
+        Quality Definition Title.
+        """
+        return pulumi.get(self, "title")
+
+
+@pulumi.output_type
 class GetDelayProfilesDelayProfileResult(dict):
     def __init__(__self__, *,
                  enable_torrent: bool,
                  enable_usenet: bool,
                  id: int,
                  order: int,
                  preferred_protocol: str,
@@ -552,76 +624,14 @@
         """
         Usenet delay.
         """
         return pulumi.get(self, "usenet_delay")
 
 
 @pulumi.output_type
-class GetMetadataProfilesMetadataProfileResult(dict):
-    def __init__(__self__, *,
-                 id: int,
-                 name: str,
-                 primary_album_types: Sequence[int],
-                 release_statuses: Sequence[int],
-                 secondary_album_types: Sequence[int]):
-        """
-        :param int id: Metadata Profile ID.
-        :param str name: Metadata Profile name.
-        :param Sequence[int] primary_album_types: Primary album types.
-        :param Sequence[int] release_statuses: Release statuses.
-        :param Sequence[int] secondary_album_types: Secondary album types.
-        """
-        pulumi.set(__self__, "id", id)
-        pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "primary_album_types", primary_album_types)
-        pulumi.set(__self__, "release_statuses", release_statuses)
-        pulumi.set(__self__, "secondary_album_types", secondary_album_types)
-
-    @property
-    @pulumi.getter
-    def id(self) -> int:
-        """
-        Metadata Profile ID.
-        """
-        return pulumi.get(self, "id")
-
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        """
-        Metadata Profile name.
-        """
-        return pulumi.get(self, "name")
-
-    @property
-    @pulumi.getter(name="primaryAlbumTypes")
-    def primary_album_types(self) -> Sequence[int]:
-        """
-        Primary album types.
-        """
-        return pulumi.get(self, "primary_album_types")
-
-    @property
-    @pulumi.getter(name="releaseStatuses")
-    def release_statuses(self) -> Sequence[int]:
-        """
-        Release statuses.
-        """
-        return pulumi.get(self, "release_statuses")
-
-    @property
-    @pulumi.getter(name="secondaryAlbumTypes")
-    def secondary_album_types(self) -> Sequence[int]:
-        """
-        Secondary album types.
-        """
-        return pulumi.get(self, "secondary_album_types")
-
-
-@pulumi.output_type
 class GetPrimaryAlbumTypesElementResult(dict):
     def __init__(__self__, *,
                  id: int,
                  name: str):
         """
         :param int id: Album type ID.
         :param str name: Album type name.
@@ -643,88 +653,15 @@
         """
         Album type name.
         """
         return pulumi.get(self, "name")
 
 
 @pulumi.output_type
-class GetQualityDefinitionsQualityDefinitionResult(dict):
-    def __init__(__self__, *,
-                 id: int,
-                 max_size: float,
-                 min_size: float,
-                 quality_id: int,
-                 quality_name: str,
-                 title: str):
-        """
-        :param int id: Quality Definition ID.
-        :param float max_size: Maximum size MB/min.
-        :param float min_size: Minimum size MB/min.
-        :param int quality_id: Quality ID.
-        :param str quality_name: Quality Name.
-        :param str title: Quality Definition Title.
-        """
-        pulumi.set(__self__, "id", id)
-        pulumi.set(__self__, "max_size", max_size)
-        pulumi.set(__self__, "min_size", min_size)
-        pulumi.set(__self__, "quality_id", quality_id)
-        pulumi.set(__self__, "quality_name", quality_name)
-        pulumi.set(__self__, "title", title)
-
-    @property
-    @pulumi.getter
-    def id(self) -> int:
-        """
-        Quality Definition ID.
-        """
-        return pulumi.get(self, "id")
-
-    @property
-    @pulumi.getter(name="maxSize")
-    def max_size(self) -> float:
-        """
-        Maximum size MB/min.
-        """
-        return pulumi.get(self, "max_size")
-
-    @property
-    @pulumi.getter(name="minSize")
-    def min_size(self) -> float:
-        """
-        Minimum size MB/min.
-        """
-        return pulumi.get(self, "min_size")
-
-    @property
-    @pulumi.getter(name="qualityId")
-    def quality_id(self) -> int:
-        """
-        Quality ID.
-        """
-        return pulumi.get(self, "quality_id")
-
-    @property
-    @pulumi.getter(name="qualityName")
-    def quality_name(self) -> str:
-        """
-        Quality Name.
-        """
-        return pulumi.get(self, "quality_name")
-
-    @property
-    @pulumi.getter
-    def title(self) -> str:
-        """
-        Quality Definition Title.
-        """
-        return pulumi.get(self, "title")
-
-
-@pulumi.output_type
-class GetQualityProfileFormatItemResult(dict):
+class GetProfileFormatItemResult(dict):
     def __init__(__self__, *,
                  format: int,
                  name: str,
                  score: int):
         """
         :param int format: Format.
         :param str name: Name.
@@ -756,23 +693,23 @@
         """
         Score.
         """
         return pulumi.get(self, "score")
 
 
 @pulumi.output_type
-class GetQualityProfileQualityGroupResult(dict):
+class GetProfileQualityGroupResult(dict):
     def __init__(__self__, *,
                  id: int,
                  name: str,
-                 qualities: Sequence['outputs.GetQualityProfileQualityGroupQualityResult']):
+                 qualities: Sequence['outputs.GetProfileQualityGroupQualityResult']):
         """
         :param int id: Quality group ID.
         :param str name: Quality group name.
-        :param Sequence['GetQualityProfileQualityGroupQualityArgs'] qualities: Qualities in group.
+        :param Sequence['GetProfileQualityGroupQualityArgs'] qualities: Qualities in group.
         """
         pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "qualities", qualities)
 
     @property
     @pulumi.getter
@@ -788,23 +725,23 @@
         """
         Quality group name.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
-    def qualities(self) -> Sequence['outputs.GetQualityProfileQualityGroupQualityResult']:
+    def qualities(self) -> Sequence['outputs.GetProfileQualityGroupQualityResult']:
         """
         Qualities in group.
         """
         return pulumi.get(self, "qualities")
 
 
 @pulumi.output_type
-class GetQualityProfileQualityGroupQualityResult(dict):
+class GetProfileQualityGroupQualityResult(dict):
     def __init__(__self__, *,
                  id: int,
                  name: str):
         """
         :param int id: Quality group ID.
         :param str name: Name.
         """
@@ -825,32 +762,32 @@
         """
         Name.
         """
         return pulumi.get(self, "name")
 
 
 @pulumi.output_type
-class GetQualityProfilesQualityProfileResult(dict):
+class GetProfilesQualityProfileResult(dict):
     def __init__(__self__, *,
                  cutoff: int,
                  cutoff_format_score: int,
-                 format_items: Sequence['outputs.GetQualityProfilesQualityProfileFormatItemResult'],
+                 format_items: Sequence['outputs.GetProfilesQualityProfileFormatItemResult'],
                  id: int,
                  min_format_score: int,
                  name: str,
-                 quality_groups: Sequence['outputs.GetQualityProfilesQualityProfileQualityGroupResult'],
+                 quality_groups: Sequence['outputs.GetProfilesQualityProfileQualityGroupResult'],
                  upgrade_allowed: bool):
         """
         :param int cutoff: Quality ID to which cutoff.
         :param int cutoff_format_score: Cutoff format score.
-        :param Sequence['GetQualityProfilesQualityProfileFormatItemArgs'] format_items: Format items.
+        :param Sequence['GetProfilesQualityProfileFormatItemArgs'] format_items: Format items.
         :param int id: Quality Profile ID.
         :param int min_format_score: Min format score.
         :param str name: Quality Profile Name.
-        :param Sequence['GetQualityProfilesQualityProfileQualityGroupArgs'] quality_groups: Quality groups.
+        :param Sequence['GetProfilesQualityProfileQualityGroupArgs'] quality_groups: Quality groups.
         :param bool upgrade_allowed: Upgrade allowed flag.
         """
         pulumi.set(__self__, "cutoff", cutoff)
         pulumi.set(__self__, "cutoff_format_score", cutoff_format_score)
         pulumi.set(__self__, "format_items", format_items)
         pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "min_format_score", min_format_score)
@@ -872,15 +809,15 @@
         """
         Cutoff format score.
         """
         return pulumi.get(self, "cutoff_format_score")
 
     @property
     @pulumi.getter(name="formatItems")
-    def format_items(self) -> Sequence['outputs.GetQualityProfilesQualityProfileFormatItemResult']:
+    def format_items(self) -> Sequence['outputs.GetProfilesQualityProfileFormatItemResult']:
         """
         Format items.
         """
         return pulumi.get(self, "format_items")
 
     @property
     @pulumi.getter
@@ -904,15 +841,15 @@
         """
         Quality Profile Name.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="qualityGroups")
-    def quality_groups(self) -> Sequence['outputs.GetQualityProfilesQualityProfileQualityGroupResult']:
+    def quality_groups(self) -> Sequence['outputs.GetProfilesQualityProfileQualityGroupResult']:
         """
         Quality groups.
         """
         return pulumi.get(self, "quality_groups")
 
     @property
     @pulumi.getter(name="upgradeAllowed")
@@ -920,15 +857,15 @@
         """
         Upgrade allowed flag.
         """
         return pulumi.get(self, "upgrade_allowed")
 
 
 @pulumi.output_type
-class GetQualityProfilesQualityProfileFormatItemResult(dict):
+class GetProfilesQualityProfileFormatItemResult(dict):
     def __init__(__self__, *,
                  format: int,
                  name: str,
                  score: int):
         """
         :param int format: Format.
         :param str name: Name.
@@ -960,23 +897,23 @@
         """
         Score.
         """
         return pulumi.get(self, "score")
 
 
 @pulumi.output_type
-class GetQualityProfilesQualityProfileQualityGroupResult(dict):
+class GetProfilesQualityProfileQualityGroupResult(dict):
     def __init__(__self__, *,
                  id: int,
                  name: str,
-                 qualities: Sequence['outputs.GetQualityProfilesQualityProfileQualityGroupQualityResult']):
+                 qualities: Sequence['outputs.GetProfilesQualityProfileQualityGroupQualityResult']):
         """
         :param int id: Quality Profile ID.
         :param str name: Name.
-        :param Sequence['GetQualityProfilesQualityProfileQualityGroupQualityArgs'] qualities: Qualities in group.
+        :param Sequence['GetProfilesQualityProfileQualityGroupQualityArgs'] qualities: Qualities in group.
         """
         pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "qualities", qualities)
 
     @property
     @pulumi.getter
@@ -992,23 +929,23 @@
         """
         Name.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
-    def qualities(self) -> Sequence['outputs.GetQualityProfilesQualityProfileQualityGroupQualityResult']:
+    def qualities(self) -> Sequence['outputs.GetProfilesQualityProfileQualityGroupQualityResult']:
         """
         Qualities in group.
         """
         return pulumi.get(self, "qualities")
 
 
 @pulumi.output_type
-class GetQualityProfilesQualityProfileQualityGroupQualityResult(dict):
+class GetProfilesQualityProfileQualityGroupQualityResult(dict):
     def __init__(__self__, *,
                  id: int,
                  name: str):
         """
         :param int id: Quality Profile ID.
         :param str name: Name.
         """
```

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/quality_definition.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/definition.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
-__all__ = ['QualityDefinitionArgs', 'QualityDefinition']
+__all__ = ['DefinitionArgs', 'Definition']
 
 @pulumi.input_type
-class QualityDefinitionArgs:
+class DefinitionArgs:
     def __init__(__self__, *,
                  title: pulumi.Input[str],
                  max_size: Optional[pulumi.Input[float]] = None,
                  min_size: Optional[pulumi.Input[float]] = None):
         """
-        The set of arguments for constructing a QualityDefinition resource.
+        The set of arguments for constructing a Definition resource.
         :param pulumi.Input[str] title: Quality Definition Title.
         :param pulumi.Input[float] max_size: Maximum size MB/min.
         :param pulumi.Input[float] min_size: Minimum size MB/min.
         """
         pulumi.set(__self__, "title", title)
         if max_size is not None:
             pulumi.set(__self__, "max_size", max_size)
@@ -63,23 +63,23 @@
 
     @min_size.setter
     def min_size(self, value: Optional[pulumi.Input[float]]):
         pulumi.set(self, "min_size", value)
 
 
 @pulumi.input_type
-class _QualityDefinitionState:
+class _DefinitionState:
     def __init__(__self__, *,
                  max_size: Optional[pulumi.Input[float]] = None,
                  min_size: Optional[pulumi.Input[float]] = None,
                  quality_id: Optional[pulumi.Input[int]] = None,
                  quality_name: Optional[pulumi.Input[str]] = None,
                  title: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering QualityDefinition resources.
+        Input properties used for looking up and filtering Definition resources.
         :param pulumi.Input[float] max_size: Maximum size MB/min.
         :param pulumi.Input[float] min_size: Minimum size MB/min.
         :param pulumi.Input[int] quality_id: Quality ID.
         :param pulumi.Input[str] quality_name: Quality Name.
         :param pulumi.Input[str] title: Quality Definition Title.
         """
         if max_size is not None:
@@ -150,15 +150,15 @@
         return pulumi.get(self, "title")
 
     @title.setter
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
 
-class QualityDefinition(pulumi.CustomResource):
+class Definition(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  max_size: Optional[pulumi.Input[float]] = None,
                  min_size: Optional[pulumi.Input[float]] = None,
                  title: Optional[pulumi.Input[str]] = None,
@@ -168,48 +168,48 @@
         For more information refer to [Quality Definition](https://wiki.servarr.com/lidarr/settings#quality-1) documentation.
 
         ## Import
 
         import using the API/UI ID
 
         ```sh
-         $ pulumi import lidarr:Profiles/qualityDefinition:QualityDefinition example 10
+         $ pulumi import lidarr:Profiles/definition:Definition example 10
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[float] max_size: Maximum size MB/min.
         :param pulumi.Input[float] min_size: Minimum size MB/min.
         :param pulumi.Input[str] title: Quality Definition Title.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: QualityDefinitionArgs,
+                 args: DefinitionArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         <!-- subcategory:Profiles -->Quality Definition resource.
         For more information refer to [Quality Definition](https://wiki.servarr.com/lidarr/settings#quality-1) documentation.
 
         ## Import
 
         import using the API/UI ID
 
         ```sh
-         $ pulumi import lidarr:Profiles/qualityDefinition:QualityDefinition example 10
+         $ pulumi import lidarr:Profiles/definition:Definition example 10
         ```
 
         :param str resource_name: The name of the resource.
-        :param QualityDefinitionArgs args: The arguments to use to populate this resource's properties.
+        :param DefinitionArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(QualityDefinitionArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(DefinitionArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -220,61 +220,61 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = QualityDefinitionArgs.__new__(QualityDefinitionArgs)
+            __props__ = DefinitionArgs.__new__(DefinitionArgs)
 
             __props__.__dict__["max_size"] = max_size
             __props__.__dict__["min_size"] = min_size
             if title is None and not opts.urn:
                 raise TypeError("Missing required property 'title'")
             __props__.__dict__["title"] = title
             __props__.__dict__["quality_id"] = None
             __props__.__dict__["quality_name"] = None
-        super(QualityDefinition, __self__).__init__(
-            'lidarr:Profiles/qualityDefinition:QualityDefinition',
+        super(Definition, __self__).__init__(
+            'lidarr:Profiles/definition:Definition',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             max_size: Optional[pulumi.Input[float]] = None,
             min_size: Optional[pulumi.Input[float]] = None,
             quality_id: Optional[pulumi.Input[int]] = None,
             quality_name: Optional[pulumi.Input[str]] = None,
-            title: Optional[pulumi.Input[str]] = None) -> 'QualityDefinition':
+            title: Optional[pulumi.Input[str]] = None) -> 'Definition':
         """
-        Get an existing QualityDefinition resource's state with the given name, id, and optional extra
+        Get an existing Definition resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[float] max_size: Maximum size MB/min.
         :param pulumi.Input[float] min_size: Minimum size MB/min.
         :param pulumi.Input[int] quality_id: Quality ID.
         :param pulumi.Input[str] quality_name: Quality Name.
         :param pulumi.Input[str] title: Quality Definition Title.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _QualityDefinitionState.__new__(_QualityDefinitionState)
+        __props__ = _DefinitionState.__new__(_DefinitionState)
 
         __props__.__dict__["max_size"] = max_size
         __props__.__dict__["min_size"] = min_size
         __props__.__dict__["quality_id"] = quality_id
         __props__.__dict__["quality_name"] = quality_name
         __props__.__dict__["title"] = title
-        return QualityDefinition(resource_name, opts=opts, __props__=__props__)
+        return Definition(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="maxSize")
     def max_size(self) -> pulumi.Output[float]:
         """
         Maximum size MB/min.
         """
```

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/profiles/release_profile.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/profiles/release_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/provider.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/system/_inputs.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/system/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/system/get_host.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/system/get_host.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/system/get_status.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/system/get_status.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/system/host.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/system/host.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/system/outputs.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/system/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/tags/get_tag.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/tags/get_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/tags/get_tags.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/tags/get_tags.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/tags/outputs.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/tags/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr/tags/tag.py` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr/tags/tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr.egg-info/PKG-INFO` & `pulumi_lidarr-2.0.0a9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi-lidarr
-Version: 2.0.0a8
+Name: pulumi_lidarr
+Version: 2.0.0a9
 Summary: A Pulumi package for creating and managing Lidarr resources
 Home-page: https://github.com/MaienM/pulumi-lidarr
 License: Apache-2.0
 Project-URL: Repository, https://github.com/MaienM/pulumi-lidarr
 Keywords: pulumi lidarr category/utility
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_lidarr-2.0.0a8/pulumi_lidarr.egg-info/SOURCES.txt` & `pulumi_lidarr-2.0.0a9/pulumi_lidarr.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -89,17 +89,20 @@
 pulumi_lidarr/mediamanagement/outputs.py
 pulumi_lidarr/mediamanagement/root_folder.py
 pulumi_lidarr/metadata/__init__.py
 pulumi_lidarr/metadata/config.py
 pulumi_lidarr/metadata/get_config.py
 pulumi_lidarr/metadata/get_consumers.py
 pulumi_lidarr/metadata/get_metadata.py
+pulumi_lidarr/metadata/get_profile.py
+pulumi_lidarr/metadata/get_profiles.py
 pulumi_lidarr/metadata/kodi.py
 pulumi_lidarr/metadata/metadata.py
 pulumi_lidarr/metadata/outputs.py
+pulumi_lidarr/metadata/profile.py
 pulumi_lidarr/metadata/roksbox.py
 pulumi_lidarr/metadata/wdtv.py
 pulumi_lidarr/notifications/__init__.py
 pulumi_lidarr/notifications/apprise.py
 pulumi_lidarr/notifications/custom_script.py
 pulumi_lidarr/notifications/discord.py
 pulumi_lidarr/notifications/email.py
@@ -126,42 +129,39 @@
 pulumi_lidarr/notifications/synology_indexer.py
 pulumi_lidarr/notifications/telegram.py
 pulumi_lidarr/notifications/twitter.py
 pulumi_lidarr/notifications/webhook.py
 pulumi_lidarr/profiles/__init__.py
 pulumi_lidarr/profiles/_inputs.py
 pulumi_lidarr/profiles/custom_format.py
+pulumi_lidarr/profiles/definition.py
 pulumi_lidarr/profiles/delay_profile.py
 pulumi_lidarr/profiles/get_condition.py
 pulumi_lidarr/profiles/get_condition_release_group.py
 pulumi_lidarr/profiles/get_condition_release_title.py
 pulumi_lidarr/profiles/get_condition_size.py
 pulumi_lidarr/profiles/get_custom_format.py
 pulumi_lidarr/profiles/get_custom_formats.py
+pulumi_lidarr/profiles/get_definition.py
+pulumi_lidarr/profiles/get_definitions.py
 pulumi_lidarr/profiles/get_delay_profile.py
 pulumi_lidarr/profiles/get_delay_profiles.py
-pulumi_lidarr/profiles/get_metadata_profile.py
-pulumi_lidarr/profiles/get_metadata_profiles.py
 pulumi_lidarr/profiles/get_primary_album_type.py
 pulumi_lidarr/profiles/get_primary_album_types.py
+pulumi_lidarr/profiles/get_profile.py
+pulumi_lidarr/profiles/get_profiles.py
 pulumi_lidarr/profiles/get_quality.py
-pulumi_lidarr/profiles/get_quality_definition.py
-pulumi_lidarr/profiles/get_quality_definitions.py
-pulumi_lidarr/profiles/get_quality_profile.py
-pulumi_lidarr/profiles/get_quality_profiles.py
 pulumi_lidarr/profiles/get_release_profile.py
 pulumi_lidarr/profiles/get_release_profiles.py
 pulumi_lidarr/profiles/get_release_status.py
 pulumi_lidarr/profiles/get_release_statuses.py
 pulumi_lidarr/profiles/get_secondary_album_type.py
 pulumi_lidarr/profiles/get_secondary_album_types.py
-pulumi_lidarr/profiles/metadata_profile.py
 pulumi_lidarr/profiles/outputs.py
-pulumi_lidarr/profiles/quality_definition.py
-pulumi_lidarr/profiles/quality_profile.py
+pulumi_lidarr/profiles/profile.py
 pulumi_lidarr/profiles/release_profile.py
 pulumi_lidarr/system/__init__.py
 pulumi_lidarr/system/_inputs.py
 pulumi_lidarr/system/get_host.py
 pulumi_lidarr/system/get_status.py
 pulumi_lidarr/system/host.py
 pulumi_lidarr/system/outputs.py
```

### Comparing `pulumi_lidarr-2.0.0a8/setup.py` & `pulumi_lidarr-2.0.0a9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import errno
 import os
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "2.0.0a8"
+VERSION = "2.0.0a9"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "lidarr Pulumi Package - Development Version"
```

