# Comparing `tmp/pulumi_docker_build-0.0.1a3.tar.gz` & `tmp/pulumi_docker_build-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_docker_build-0.0.1a3.tar", last modified: Wed Apr 17 19:52:01 2024, max compression
+gzip compressed data, was "pulumi_docker_build-0.0.2.tar", last modified: Thu Apr 25 17:31:24 2024, max compression
```

## Comparing `pulumi_docker_build-0.0.1a3.tar` & `pulumi_docker_build-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-17 19:52:01.817405 pulumi_docker_build-0.0.1a3/
--rw-r--r--   0 runner    (1000) runner    (1000)     4788 2024-04-17 19:52:01.817405 pulumi_docker_build-0.0.1a3/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     4355 2024-04-17 19:51:50.000000 pulumi_docker_build-0.0.1a3/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-17 19:52:01.817405 pulumi_docker_build-0.0.1a3/pulumi_docker_build/
--rw-------   0 runner    (1000) runner    (1000)      983 2024-04-17 19:51:50.000000 pulumi_docker_build-0.0.1a3/pulumi_docker_build/__init__.py
--rw-------   0 runner    (1000) runner    (1000)     1928 2024-04-17 19:51:50.000000 pulumi_docker_build-0.0.1a3/pulumi_docker_build/_enums.py
--rw-------   0 runner    (1000) runner    (1000)    97964 2024-04-17 19:51:50.000000 pulumi_docker_build-0.0.1a3/pulumi_docker_build/_inputs.py
--rw-------   0 runner    (1000) runner    (1000)     9265 2024-04-17 19:51:50.000000 pulumi_docker_build-0.0.1a3/pulumi_docker_build/_utilities.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-17 19:52:01.817405 pulumi_docker_build-0.0.1a3/pulumi_docker_build/config/
--rw-------   0 runner    (1000) runner    (1000)      267 2024-04-17 19:51:50.000000 pulumi_docker_build-0.0.1a3/pulumi_docker_build/config/__init__.py
--rw-------   0 runner    (1000) runner    (1000)      441 2024-04-17 19:51:50.000000 pulumi_docker_build-0.0.1a3/pulumi_docker_build/config/__init__.pyi
--rw-------   0 runner    (1000) runner    (1000)      756 2024-04-17 19:51:50.000000 pulumi_docker_build-0.0.1a3/pulumi_docker_build/config/vars.py
--rw-------   0 runner    (1000) runner    (1000)    76626 2024-04-17 19:51:50.000000 pulumi_docker_build-0.0.1a3/pulumi_docker_build/image.py
--rw-------   0 runner    (1000) runner    (1000)    13254 2024-04-17 19:51:50.000000 pulumi_docker_build-0.0.1a3/pulumi_docker_build/index.py
--rw-------   0 runner    (1000) runner    (1000)    83253 2024-04-17 19:51:50.000000 pulumi_docker_build-0.0.1a3/pulumi_docker_build/outputs.py
--rw-------   0 runner    (1000) runner    (1000)     4780 2024-04-17 19:51:50.000000 pulumi_docker_build-0.0.1a3/pulumi_docker_build/provider.py
--rw-------   0 runner    (1000) runner    (1000)      102 2024-04-17 19:51:50.000000 pulumi_docker_build-0.0.1a3/pulumi_docker_build/pulumi-plugin.json
--rw-------   0 runner    (1000) runner    (1000)        0 2024-04-17 19:51:50.000000 pulumi_docker_build-0.0.1a3/pulumi_docker_build/py.typed
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-17 19:52:01.817405 pulumi_docker_build-0.0.1a3/pulumi_docker_build.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     4788 2024-04-17 19:52:01.000000 pulumi_docker_build-0.0.1a3/pulumi_docker_build.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      668 2024-04-17 19:52:01.000000 pulumi_docker_build-0.0.1a3/pulumi_docker_build.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-17 19:52:01.000000 pulumi_docker_build-0.0.1a3/pulumi_docker_build.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       49 2024-04-17 19:52:01.000000 pulumi_docker_build-0.0.1a3/pulumi_docker_build.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       20 2024-04-17 19:52:01.000000 pulumi_docker_build-0.0.1a3/pulumi_docker_build.egg-info/top_level.txt
--rw-------   0 runner    (1000) runner    (1000)      669 2024-04-17 19:51:50.000000 pulumi_docker_build-0.0.1a3/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-04-17 19:52:01.817405 pulumi_docker_build-0.0.1a3/setup.cfg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-25 17:31:24.462243 pulumi_docker_build-0.0.2/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2543 2024-04-25 17:31:24.462243 pulumi_docker_build-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     2057 2024-04-25 17:31:16.000000 pulumi_docker_build-0.0.2/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-25 17:31:24.462243 pulumi_docker_build-0.0.2/pulumi_docker_build/
+-rw-------   0 runner    (1000) runner    (1000)      983 2024-04-25 17:31:16.000000 pulumi_docker_build-0.0.2/pulumi_docker_build/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     1928 2024-04-25 17:31:16.000000 pulumi_docker_build-0.0.2/pulumi_docker_build/_enums.py
+-rw-------   0 runner    (1000) runner    (1000)    97964 2024-04-25 17:31:16.000000 pulumi_docker_build-0.0.2/pulumi_docker_build/_inputs.py
+-rw-------   0 runner    (1000) runner    (1000)     9230 2024-04-25 17:31:16.000000 pulumi_docker_build-0.0.2/pulumi_docker_build/_utilities.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-25 17:31:24.462243 pulumi_docker_build-0.0.2/pulumi_docker_build/config/
+-rw-------   0 runner    (1000) runner    (1000)      267 2024-04-25 17:31:16.000000 pulumi_docker_build-0.0.2/pulumi_docker_build/config/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)      441 2024-04-25 17:31:16.000000 pulumi_docker_build-0.0.2/pulumi_docker_build/config/__init__.pyi
+-rw-------   0 runner    (1000) runner    (1000)      756 2024-04-25 17:31:16.000000 pulumi_docker_build-0.0.2/pulumi_docker_build/config/vars.py
+-rw-------   0 runner    (1000) runner    (1000)    75687 2024-04-25 17:31:16.000000 pulumi_docker_build-0.0.2/pulumi_docker_build/image.py
+-rw-------   0 runner    (1000) runner    (1000)    14598 2024-04-25 17:31:16.000000 pulumi_docker_build-0.0.2/pulumi_docker_build/index.py
+-rw-------   0 runner    (1000) runner    (1000)    83253 2024-04-25 17:31:16.000000 pulumi_docker_build-0.0.2/pulumi_docker_build/outputs.py
+-rw-------   0 runner    (1000) runner    (1000)     4780 2024-04-25 17:31:16.000000 pulumi_docker_build-0.0.2/pulumi_docker_build/provider.py
+-rw-------   0 runner    (1000) runner    (1000)       49 2024-04-25 17:31:16.000000 pulumi_docker_build-0.0.2/pulumi_docker_build/pulumi-plugin.json
+-rw-------   0 runner    (1000) runner    (1000)        0 2024-04-25 17:31:16.000000 pulumi_docker_build-0.0.2/pulumi_docker_build/py.typed
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-25 17:31:24.462243 pulumi_docker_build-0.0.2/pulumi_docker_build.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2543 2024-04-25 17:31:24.000000 pulumi_docker_build-0.0.2/pulumi_docker_build.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      668 2024-04-25 17:31:24.000000 pulumi_docker_build-0.0.2/pulumi_docker_build.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-25 17:31:24.000000 pulumi_docker_build-0.0.2/pulumi_docker_build.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       49 2024-04-25 17:31:24.000000 pulumi_docker_build-0.0.2/pulumi_docker_build.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       20 2024-04-25 17:31:24.000000 pulumi_docker_build-0.0.2/pulumi_docker_build.egg-info/top_level.txt
+-rw-------   0 runner    (1000) runner    (1000)      725 2024-04-25 17:31:16.000000 pulumi_docker_build-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-04-25 17:31:24.462243 pulumi_docker_build-0.0.2/setup.cfg
```

### Comparing `pulumi_docker_build-0.0.1a3/pulumi_docker_build/__init__.py` & `pulumi_docker_build-0.0.2/pulumi_docker_build/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.0.1a3/pulumi_docker_build/_enums.py` & `pulumi_docker_build-0.0.2/pulumi_docker_build/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.0.1a3/pulumi_docker_build/_inputs.py` & `pulumi_docker_build-0.0.2/pulumi_docker_build/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.0.1a3/pulumi_docker_build/_utilities.py` & `pulumi_docker_build-0.0.2/pulumi_docker_build/_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,8 +284,8 @@
         await o._future,
         await o._is_known,
         await o._is_secret,
         await o._resources,
     )
 
 def get_plugin_download_url():
-	return "github.com/pulumi/pulumi-docker-build"
+	return None
```

### Comparing `pulumi_docker_build-0.0.1a3/pulumi_docker_build/config/vars.py` & `pulumi_docker_build-0.0.2/pulumi_docker_build/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.0.1a3/pulumi_docker_build/image.py` & `pulumi_docker_build-0.0.2/pulumi_docker_build/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from ._inputs import *
 
 __all__ = ['ImageArgs', 'Image']
 
 @pulumi.input_type
 class ImageArgs:
     def __init__(__self__, *,
+                 push: pulumi.Input[bool],
                  add_hosts: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  build_args: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  build_on_preview: Optional[pulumi.Input[bool]] = None,
                  builder: Optional[pulumi.Input['BuilderConfigArgs']] = None,
                  cache_from: Optional[pulumi.Input[Sequence[pulumi.Input['CacheFromArgs']]]] = None,
                  cache_to: Optional[pulumi.Input[Sequence[pulumi.Input['CacheToArgs']]]] = None,
                  context: Optional[pulumi.Input['BuildContextArgs']] = None,
@@ -29,48 +30,49 @@
                  exports: Optional[pulumi.Input[Sequence[pulumi.Input['ExportArgs']]]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  load: Optional[pulumi.Input[bool]] = None,
                  network: Optional[pulumi.Input['NetworkMode']] = None,
                  no_cache: Optional[pulumi.Input[bool]] = None,
                  platforms: Optional[pulumi.Input[Sequence[pulumi.Input['Platform']]]] = None,
                  pull: Optional[pulumi.Input[bool]] = None,
-                 push: Optional[pulumi.Input[bool]] = None,
                  registries: Optional[pulumi.Input[Sequence[pulumi.Input['RegistryArgs']]]] = None,
                  secrets: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  ssh: Optional[pulumi.Input[Sequence[pulumi.Input['SSHArgs']]]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  target: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Image resource.
+        :param pulumi.Input[bool] push: When `true` the build will automatically include a `registry` export.
+               
+               Defaults to `false`.
+               
+               Equivalent to Docker's `--push` flag.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] add_hosts: Custom `host:ip` mappings to use during the build.
                
                Equivalent to Docker's `--add-host` flag.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] build_args: `ARG` names and values to set during the build.
                
                These variables are accessed like environment variables inside `RUN`
                instructions.
                
                Build arguments are persisted in the image, so you should use `secrets`
                if these arguments are sensitive.
                
                Equivalent to Docker's `--build-arg` flag.
-        :param pulumi.Input[bool] build_on_preview: By default, preview behavior depends on the execution environment. If
-               Pulumi detects the operation is running on a CI system (GitHub Actions,
-               Travis CI, Azure Pipelines, etc.) then it will build images during
-               previews as a safeguard. Otherwise, if not running on CI, previews will
-               not build images.
-               
-               Setting this to `false` forces previews to never perform builds, and
-               setting it to `true` will always build the image during previews.
+        :param pulumi.Input[bool] build_on_preview: Setting this to `false` will always skip image builds during previews,
+               and setting it to `true` will always build images during previews.
                
                Images built during previews are never exported to registries, however
                cache manifests are still exported.
                
                On-disk Dockerfiles are always validated for syntactic correctness
                regardless of this setting.
+               
+               Defaults to `true` as a safeguard against broken images merging as part
+               of CI pipelines.
         :param pulumi.Input['BuilderConfigArgs'] builder: Builder configuration.
         :param pulumi.Input[Sequence[pulumi.Input['CacheFromArgs']]] cache_from: Cache export configuration.
                
                Equivalent to Docker's `--cache-from` flag.
         :param pulumi.Input[Sequence[pulumi.Input['CacheToArgs']]] cache_to: Cache import configuration.
                
                Equivalent to Docker's `--cache-to` flag.
@@ -127,19 +129,14 @@
                Equivalent to Docker's `--no-cache` flag.
         :param pulumi.Input[Sequence[pulumi.Input['Platform']]] platforms: Set target platform(s) for the build. Defaults to the host's platform.
                
                Equivalent to Docker's `--platform` flag.
         :param pulumi.Input[bool] pull: Always pull referenced images.
                
                Equivalent to Docker's `--pull` flag.
-        :param pulumi.Input[bool] push: When `true` the build will automatically include a `registry` export.
-               
-               Defaults to `false`.
-               
-               Equivalent to Docker's `--push` flag.
         :param pulumi.Input[Sequence[pulumi.Input['RegistryArgs']]] registries: Registry credentials. Required if reading or exporting to private
                repositories.
                
                Credentials are kept in-memory and do not pollute pre-existing
                credentials on the host.
                
                Similar to `docker login`.
@@ -163,18 +160,21 @@
                Equivalent to Docker's `--tag` flag.
         :param pulumi.Input[str] target: Set the target build stage(s) to build.
                
                If not specified all targets will be built by default.
                
                Equivalent to Docker's `--target` flag.
         """
+        pulumi.set(__self__, "push", push)
         if add_hosts is not None:
             pulumi.set(__self__, "add_hosts", add_hosts)
         if build_args is not None:
             pulumi.set(__self__, "build_args", build_args)
+        if build_on_preview is None:
+            build_on_preview = True
         if build_on_preview is not None:
             pulumi.set(__self__, "build_on_preview", build_on_preview)
         if builder is not None:
             pulumi.set(__self__, "builder", builder)
         if cache_from is not None:
             pulumi.set(__self__, "cache_from", cache_from)
         if cache_to is not None:
@@ -197,28 +197,42 @@
             pulumi.set(__self__, "network", network)
         if no_cache is not None:
             pulumi.set(__self__, "no_cache", no_cache)
         if platforms is not None:
             pulumi.set(__self__, "platforms", platforms)
         if pull is not None:
             pulumi.set(__self__, "pull", pull)
-        if push is not None:
-            pulumi.set(__self__, "push", push)
         if registries is not None:
             pulumi.set(__self__, "registries", registries)
         if secrets is not None:
             pulumi.set(__self__, "secrets", secrets)
         if ssh is not None:
             pulumi.set(__self__, "ssh", ssh)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if target is not None:
             pulumi.set(__self__, "target", target)
 
     @property
+    @pulumi.getter
+    def push(self) -> pulumi.Input[bool]:
+        """
+        When `true` the build will automatically include a `registry` export.
+
+        Defaults to `false`.
+
+        Equivalent to Docker's `--push` flag.
+        """
+        return pulumi.get(self, "push")
+
+    @push.setter
+    def push(self, value: pulumi.Input[bool]):
+        pulumi.set(self, "push", value)
+
+    @property
     @pulumi.getter(name="addHosts")
     def add_hosts(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         Custom `host:ip` mappings to use during the build.
 
         Equivalent to Docker's `--add-host` flag.
         """
@@ -248,28 +262,25 @@
     def build_args(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "build_args", value)
 
     @property
     @pulumi.getter(name="buildOnPreview")
     def build_on_preview(self) -> Optional[pulumi.Input[bool]]:
         """
-        By default, preview behavior depends on the execution environment. If
-        Pulumi detects the operation is running on a CI system (GitHub Actions,
-        Travis CI, Azure Pipelines, etc.) then it will build images during
-        previews as a safeguard. Otherwise, if not running on CI, previews will
-        not build images.
-
-        Setting this to `false` forces previews to never perform builds, and
-        setting it to `true` will always build the image during previews.
+        Setting this to `false` will always skip image builds during previews,
+        and setting it to `true` will always build images during previews.
 
         Images built during previews are never exported to registries, however
         cache manifests are still exported.
 
         On-disk Dockerfiles are always validated for syntactic correctness
         regardless of this setting.
+
+        Defaults to `true` as a safeguard against broken images merging as part
+        of CI pipelines.
         """
         return pulumi.get(self, "build_on_preview")
 
     @build_on_preview.setter
     def build_on_preview(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "build_on_preview", value)
 
@@ -478,30 +489,14 @@
 
     @pull.setter
     def pull(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "pull", value)
 
     @property
     @pulumi.getter
-    def push(self) -> Optional[pulumi.Input[bool]]:
-        """
-        When `true` the build will automatically include a `registry` export.
-
-        Defaults to `false`.
-
-        Equivalent to Docker's `--push` flag.
-        """
-        return pulumi.get(self, "push")
-
-    @push.setter
-    def push(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "push", value)
-
-    @property
-    @pulumi.getter
     def registries(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['RegistryArgs']]]]:
         """
         Registry credentials. Required if reading or exporting to private
         repositories.
 
         Credentials are kept in-memory and do not pollute pre-existing
         credentials on the host.
@@ -612,54 +607,46 @@
                  __props__=None):
         """
         A Docker image built using buildx -- Docker's interface to the improved
         BuildKit backend.
 
         ## Stability
 
-        **This resource is experimental and subject to change.**
-
-        API types are unstable. Subsequent releases _may_ require manual edits
-        to your state file(s) in order to adopt API changes.
-
-        `retainOnDelete: true` is recommended with this resource until it is
-        stable. This enables future API changes to be adopted more easily by renaming
-        resources.
+        **This resource is pre-1.0 and in public preview.**
 
-        Only use this resource if you understand and accept the risks.
+        We will strive to keep APIs and behavior as stable as possible, but we
+        cannot guarantee stability until version 1.0.
 
-        ## Migrating v3 and v4 Image resources
+        ## Migrating Pulumi Docker v3 and v4 Image resources
 
-        The `Image` resource provides a superset of functionality over the `Image` resources available in versions 3 and 4 of the Pulumi Docker provider.
+        This provider's `Image` resource provides a superset of functionality over the `Image` resources available in versions 3 and 4 of the Pulumi Docker provider.
         Existing `Image` resources can be converted to the docker-build `Image` resources with minor modifications.
 
         ### Behavioral differences
 
         There are several key behavioral differences to keep in mind when transitioning images to the new `Image` resource.
 
         #### Previews
 
         Version `3.x` of the Pulumi Docker provider always builds images during preview operations.
         This is helpful as a safeguard to prevent "broken" images from merging, but users found the behavior unnecessarily redundant when running previews and updates locally.
 
         Version `4.x` changed build-on-preview behavior to be opt-in.
         By default, `v4.x` `Image` resources do _not_ build during previews, but this behavior can be toggled with the `buildOnPreview` option.
-        Some users felt this made previews in CI less helpful because they no longer detected bad images by default.
+        Several users reported outages due to the default behavior allowing bad images to accidentally sneak through CI.
 
-        The default behavior of the `Image` resource has been changed to strike a better balance between CI use cases and manual updates.
-        By default, Pulumi will now only build `Image` resources during previews when it detects a CI environment like GitHub Actions.
-        Previews run in non-CI environments will not build images.
-        This behavior is still configurable with `buildOnPreview`.
+        The default behavior of this provider's `Image` resource is similar to `3.x` and will build images during previews.
+        This behavior can be changed by specifying `buildOnPreview`.
 
         #### Push behavior
 
         Versions `3.x` and `4.x` of the Pulumi Docker provider attempt to push images to remote registries by default.
         They expose a `skipPush: true` option to disable pushing.
 
-        The `Image` resource matches the Docker CLI's behavior and does not push images anywhere by default.
+        This provider's `Image` resource matches the Docker CLI's behavior and does not push images anywhere by default.
 
         To push images to a registry you can include `push: true` (equivalent to Docker's `--push` flag) or configure an `export` of type `registry` (equivalent to Docker's `--output type=registry`).
         Like Docker, if an image is configured without exports you will see a warning with instructions for how to enable pushing, but the build will still proceed normally.
 
         #### Secrets
 
         Version `3.x` of the Pulumi Docker provider supports secrets by way of the `extraOptions` field.
@@ -722,199 +709,211 @@
         ## Example Usage
 
         ## Example Usage
         ### Push to AWS ECR with caching
         ```python
         import pulumi
         import pulumi_aws as aws
-        import pulumi_dockerbuild as dockerbuild
+        import pulumi_docker_build as docker_build
 
         ecr_repository = aws.ecr.Repository("ecr-repository")
         auth_token = aws.ecr.get_authorization_token_output(registry_id=ecr_repository.registry_id)
-        my_image = dockerbuild.Image("my-image",
-            cache_from=[dockerbuild.CacheFromArgs(
-                registry=dockerbuild.CacheFromRegistryArgs(
+        my_image = docker_build.Image("my-image",
+            cache_from=[docker_build.CacheFromArgs(
+                registry=docker_build.CacheFromRegistryArgs(
                     ref=ecr_repository.repository_url.apply(lambda repository_url: f"{repository_url}:cache"),
                 ),
             )],
-            cache_to=[dockerbuild.CacheToArgs(
-                registry=dockerbuild.CacheToRegistryArgs(
+            cache_to=[docker_build.CacheToArgs(
+                registry=docker_build.CacheToRegistryArgs(
                     image_manifest=True,
                     oci_media_types=True,
                     ref=ecr_repository.repository_url.apply(lambda repository_url: f"{repository_url}:cache"),
                 ),
             )],
-            context=dockerbuild.BuildContextArgs(
+            context=docker_build.BuildContextArgs(
                 location="./app",
             ),
             push=True,
-            registries=[dockerbuild.RegistryArgs(
+            registries=[docker_build.RegistryArgs(
                 address=ecr_repository.repository_url,
                 password=auth_token.password,
                 username=auth_token.user_name,
             )],
             tags=[ecr_repository.repository_url.apply(lambda repository_url: f"{repository_url}:latest")])
         pulumi.export("ref", my_image.ref)
         ```
         ### Multi-platform image
         ```python
         import pulumi
-        import pulumi_dockerbuild as dockerbuild
+        import pulumi_docker_build as docker_build
 
-        image = dockerbuild.Image("image",
-            context=dockerbuild.BuildContextArgs(
+        image = docker_build.Image("image",
+            context=docker_build.BuildContextArgs(
                 location="app",
             ),
             platforms=[
-                dockerbuild.Platform.PLAN9_AMD64,
-                dockerbuild.Platform.PLAN9_386,
-            ])
+                docker_build.Platform.PLAN9_AMD64,
+                docker_build.Platform.PLAN9_386,
+            ],
+            push=False)
         ```
         ### Registry export
         ```python
         import pulumi
-        import pulumi_dockerbuild as dockerbuild
+        import pulumi_docker_build as docker_build
 
-        image = dockerbuild.Image("image",
-            context=dockerbuild.BuildContextArgs(
+        image = docker_build.Image("image",
+            context=docker_build.BuildContextArgs(
                 location="app",
             ),
             push=True,
-            registries=[dockerbuild.RegistryArgs(
+            registries=[docker_build.RegistryArgs(
                 address="docker.io",
                 password=docker_hub_password,
                 username="pulumibot",
             )],
             tags=["docker.io/pulumi/pulumi:3.107.0"])
         pulumi.export("ref", my_image["ref"])
         ```
         ### Caching
         ```python
         import pulumi
-        import pulumi_dockerbuild as dockerbuild
+        import pulumi_docker_build as docker_build
 
-        image = dockerbuild.Image("image",
-            cache_from=[dockerbuild.CacheFromArgs(
-                local=dockerbuild.CacheFromLocalArgs(
+        image = docker_build.Image("image",
+            cache_from=[docker_build.CacheFromArgs(
+                local=docker_build.CacheFromLocalArgs(
                     src="tmp/cache",
                 ),
             )],
-            cache_to=[dockerbuild.CacheToArgs(
-                local=dockerbuild.CacheToLocalArgs(
+            cache_to=[docker_build.CacheToArgs(
+                local=docker_build.CacheToLocalArgs(
                     dest="tmp/cache",
-                    mode=dockerbuild.CacheMode.MAX,
+                    mode=docker_build.CacheMode.MAX,
                 ),
             )],
-            context=dockerbuild.BuildContextArgs(
+            context=docker_build.BuildContextArgs(
                 location="app",
-            ))
+            ),
+            push=False)
         ```
         ### Docker Build Cloud
         ```python
         import pulumi
-        import pulumi_dockerbuild as dockerbuild
+        import pulumi_docker_build as docker_build
 
-        image = dockerbuild.Image("image",
-            builder=dockerbuild.BuilderConfigArgs(
+        image = docker_build.Image("image",
+            builder=docker_build.BuilderConfigArgs(
                 name="cloud-builder-name",
             ),
-            context=dockerbuild.BuildContextArgs(
+            context=docker_build.BuildContextArgs(
                 location="app",
             ),
-            exec_=True)
+            exec_=True,
+            push=False)
         ```
         ### Build arguments
         ```python
         import pulumi
-        import pulumi_dockerbuild as dockerbuild
+        import pulumi_docker_build as docker_build
 
-        image = dockerbuild.Image("image",
+        image = docker_build.Image("image",
             build_args={
                 "SET_ME_TO_TRUE": "true",
             },
-            context=dockerbuild.BuildContextArgs(
+            context=docker_build.BuildContextArgs(
                 location="app",
-            ))
+            ),
+            push=False)
         ```
         ### Build target
         ```python
         import pulumi
-        import pulumi_dockerbuild as dockerbuild
+        import pulumi_docker_build as docker_build
 
-        image = dockerbuild.Image("image",
-            context=dockerbuild.BuildContextArgs(
+        image = docker_build.Image("image",
+            context=docker_build.BuildContextArgs(
                 location="app",
             ),
+            push=False,
             target="build-me")
         ```
         ### Named contexts
         ```python
         import pulumi
-        import pulumi_dockerbuild as dockerbuild
+        import pulumi_docker_build as docker_build
 
-        image = dockerbuild.Image("image", context=dockerbuild.BuildContextArgs(
-            location="app",
-            named={
-                "golang:latest": dockerbuild.ContextArgs(
-                    location="docker-image://golang@sha256:b8e62cf593cdaff36efd90aa3a37de268e6781a2e68c6610940c48f7cdf36984",
-                ),
-            },
-        ))
+        image = docker_build.Image("image",
+            context=docker_build.BuildContextArgs(
+                location="app",
+                named={
+                    "golang:latest": docker_build.ContextArgs(
+                        location="docker-image://golang@sha256:b8e62cf593cdaff36efd90aa3a37de268e6781a2e68c6610940c48f7cdf36984",
+                    ),
+                },
+            ),
+            push=False)
         ```
         ### Remote context
         ```python
         import pulumi
-        import pulumi_dockerbuild as dockerbuild
+        import pulumi_docker_build as docker_build
 
-        image = dockerbuild.Image("image", context=dockerbuild.BuildContextArgs(
-            location="https://raw.githubusercontent.com/pulumi/pulumi-docker/api-types/provider/testdata/Dockerfile",
-        ))
+        image = docker_build.Image("image",
+            context=docker_build.BuildContextArgs(
+                location="https://raw.githubusercontent.com/pulumi/pulumi-docker/api-types/provider/testdata/Dockerfile",
+            ),
+            push=False)
         ```
         ### Inline Dockerfile
         ```python
         import pulumi
-        import pulumi_dockerbuild as dockerbuild
+        import pulumi_docker_build as docker_build
 
-        image = dockerbuild.Image("image",
-            context=dockerbuild.BuildContextArgs(
+        image = docker_build.Image("image",
+            context=docker_build.BuildContextArgs(
                 location="app",
             ),
-            dockerfile=dockerbuild.DockerfileArgs(
+            dockerfile=docker_build.DockerfileArgs(
                 inline=\"\"\"FROM busybox
         COPY hello.c ./
         \"\"\",
-            ))
+            ),
+            push=False)
         ```
         ### Remote context
         ```python
         import pulumi
-        import pulumi_dockerbuild as dockerbuild
+        import pulumi_docker_build as docker_build
 
-        image = dockerbuild.Image("image",
-            context=dockerbuild.BuildContextArgs(
+        image = docker_build.Image("image",
+            context=docker_build.BuildContextArgs(
                 location="https://github.com/docker-library/hello-world.git",
             ),
-            dockerfile=dockerbuild.DockerfileArgs(
+            dockerfile=docker_build.DockerfileArgs(
                 location="app/Dockerfile",
-            ))
+            ),
+            push=False)
         ```
         ### Local export
         ```python
         import pulumi
-        import pulumi_dockerbuild as dockerbuild
+        import pulumi_docker_build as docker_build
 
-        image = dockerbuild.Image("image",
-            context=dockerbuild.BuildContextArgs(
+        image = docker_build.Image("image",
+            context=docker_build.BuildContextArgs(
                 location="app",
             ),
-            exports=[dockerbuild.ExportArgs(
-                docker=dockerbuild.ExportDockerArgs(
+            exports=[docker_build.ExportArgs(
+                docker=docker_build.ExportDockerArgs(
                     tar=True,
                 ),
-            )])
+            )],
+            push=False)
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] add_hosts: Custom `host:ip` mappings to use during the build.
                
                Equivalent to Docker's `--add-host` flag.
@@ -923,28 +922,25 @@
                These variables are accessed like environment variables inside `RUN`
                instructions.
                
                Build arguments are persisted in the image, so you should use `secrets`
                if these arguments are sensitive.
                
                Equivalent to Docker's `--build-arg` flag.
-        :param pulumi.Input[bool] build_on_preview: By default, preview behavior depends on the execution environment. If
-               Pulumi detects the operation is running on a CI system (GitHub Actions,
-               Travis CI, Azure Pipelines, etc.) then it will build images during
-               previews as a safeguard. Otherwise, if not running on CI, previews will
-               not build images.
-               
-               Setting this to `false` forces previews to never perform builds, and
-               setting it to `true` will always build the image during previews.
+        :param pulumi.Input[bool] build_on_preview: Setting this to `false` will always skip image builds during previews,
+               and setting it to `true` will always build images during previews.
                
                Images built during previews are never exported to registries, however
                cache manifests are still exported.
                
                On-disk Dockerfiles are always validated for syntactic correctness
                regardless of this setting.
+               
+               Defaults to `true` as a safeguard against broken images merging as part
+               of CI pipelines.
         :param pulumi.Input[pulumi.InputType['BuilderConfigArgs']] builder: Builder configuration.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CacheFromArgs']]]] cache_from: Cache export configuration.
                
                Equivalent to Docker's `--cache-from` flag.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CacheToArgs']]]] cache_to: Cache import configuration.
                
                Equivalent to Docker's `--cache-to` flag.
@@ -1041,62 +1037,54 @@
                
                Equivalent to Docker's `--target` flag.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[ImageArgs] = None,
+                 args: ImageArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         A Docker image built using buildx -- Docker's interface to the improved
         BuildKit backend.
 
         ## Stability
 
-        **This resource is experimental and subject to change.**
-
-        API types are unstable. Subsequent releases _may_ require manual edits
-        to your state file(s) in order to adopt API changes.
-
-        `retainOnDelete: true` is recommended with this resource until it is
-        stable. This enables future API changes to be adopted more easily by renaming
-        resources.
+        **This resource is pre-1.0 and in public preview.**
 
-        Only use this resource if you understand and accept the risks.
+        We will strive to keep APIs and behavior as stable as possible, but we
+        cannot guarantee stability until version 1.0.
 
-        ## Migrating v3 and v4 Image resources
+        ## Migrating Pulumi Docker v3 and v4 Image resources
 
-        The `Image` resource provides a superset of functionality over the `Image` resources available in versions 3 and 4 of the Pulumi Docker provider.
+        This provider's `Image` resource provides a superset of functionality over the `Image` resources available in versions 3 and 4 of the Pulumi Docker provider.
         Existing `Image` resources can be converted to the docker-build `Image` resources with minor modifications.
 
         ### Behavioral differences
 
         There are several key behavioral differences to keep in mind when transitioning images to the new `Image` resource.
 
         #### Previews
 
         Version `3.x` of the Pulumi Docker provider always builds images during preview operations.
         This is helpful as a safeguard to prevent "broken" images from merging, but users found the behavior unnecessarily redundant when running previews and updates locally.
 
         Version `4.x` changed build-on-preview behavior to be opt-in.
         By default, `v4.x` `Image` resources do _not_ build during previews, but this behavior can be toggled with the `buildOnPreview` option.
-        Some users felt this made previews in CI less helpful because they no longer detected bad images by default.
+        Several users reported outages due to the default behavior allowing bad images to accidentally sneak through CI.
 
-        The default behavior of the `Image` resource has been changed to strike a better balance between CI use cases and manual updates.
-        By default, Pulumi will now only build `Image` resources during previews when it detects a CI environment like GitHub Actions.
-        Previews run in non-CI environments will not build images.
-        This behavior is still configurable with `buildOnPreview`.
+        The default behavior of this provider's `Image` resource is similar to `3.x` and will build images during previews.
+        This behavior can be changed by specifying `buildOnPreview`.
 
         #### Push behavior
 
         Versions `3.x` and `4.x` of the Pulumi Docker provider attempt to push images to remote registries by default.
         They expose a `skipPush: true` option to disable pushing.
 
-        The `Image` resource matches the Docker CLI's behavior and does not push images anywhere by default.
+        This provider's `Image` resource matches the Docker CLI's behavior and does not push images anywhere by default.
 
         To push images to a registry you can include `push: true` (equivalent to Docker's `--push` flag) or configure an `export` of type `registry` (equivalent to Docker's `--output type=registry`).
         Like Docker, if an image is configured without exports you will see a warning with instructions for how to enable pushing, but the build will still proceed normally.
 
         #### Secrets
 
         Version `3.x` of the Pulumi Docker provider supports secrets by way of the `extraOptions` field.
@@ -1159,199 +1147,211 @@
         ## Example Usage
 
         ## Example Usage
         ### Push to AWS ECR with caching
         ```python
         import pulumi
         import pulumi_aws as aws
-        import pulumi_dockerbuild as dockerbuild
+        import pulumi_docker_build as docker_build
 
         ecr_repository = aws.ecr.Repository("ecr-repository")
         auth_token = aws.ecr.get_authorization_token_output(registry_id=ecr_repository.registry_id)
-        my_image = dockerbuild.Image("my-image",
-            cache_from=[dockerbuild.CacheFromArgs(
-                registry=dockerbuild.CacheFromRegistryArgs(
+        my_image = docker_build.Image("my-image",
+            cache_from=[docker_build.CacheFromArgs(
+                registry=docker_build.CacheFromRegistryArgs(
                     ref=ecr_repository.repository_url.apply(lambda repository_url: f"{repository_url}:cache"),
                 ),
             )],
-            cache_to=[dockerbuild.CacheToArgs(
-                registry=dockerbuild.CacheToRegistryArgs(
+            cache_to=[docker_build.CacheToArgs(
+                registry=docker_build.CacheToRegistryArgs(
                     image_manifest=True,
                     oci_media_types=True,
                     ref=ecr_repository.repository_url.apply(lambda repository_url: f"{repository_url}:cache"),
                 ),
             )],
-            context=dockerbuild.BuildContextArgs(
+            context=docker_build.BuildContextArgs(
                 location="./app",
             ),
             push=True,
-            registries=[dockerbuild.RegistryArgs(
+            registries=[docker_build.RegistryArgs(
                 address=ecr_repository.repository_url,
                 password=auth_token.password,
                 username=auth_token.user_name,
             )],
             tags=[ecr_repository.repository_url.apply(lambda repository_url: f"{repository_url}:latest")])
         pulumi.export("ref", my_image.ref)
         ```
         ### Multi-platform image
         ```python
         import pulumi
-        import pulumi_dockerbuild as dockerbuild
+        import pulumi_docker_build as docker_build
 
-        image = dockerbuild.Image("image",
-            context=dockerbuild.BuildContextArgs(
+        image = docker_build.Image("image",
+            context=docker_build.BuildContextArgs(
                 location="app",
             ),
             platforms=[
-                dockerbuild.Platform.PLAN9_AMD64,
-                dockerbuild.Platform.PLAN9_386,
-            ])
+                docker_build.Platform.PLAN9_AMD64,
+                docker_build.Platform.PLAN9_386,
+            ],
+            push=False)
         ```
         ### Registry export
         ```python
         import pulumi
-        import pulumi_dockerbuild as dockerbuild
+        import pulumi_docker_build as docker_build
 
-        image = dockerbuild.Image("image",
-            context=dockerbuild.BuildContextArgs(
+        image = docker_build.Image("image",
+            context=docker_build.BuildContextArgs(
                 location="app",
             ),
             push=True,
-            registries=[dockerbuild.RegistryArgs(
+            registries=[docker_build.RegistryArgs(
                 address="docker.io",
                 password=docker_hub_password,
                 username="pulumibot",
             )],
             tags=["docker.io/pulumi/pulumi:3.107.0"])
         pulumi.export("ref", my_image["ref"])
         ```
         ### Caching
         ```python
         import pulumi
-        import pulumi_dockerbuild as dockerbuild
+        import pulumi_docker_build as docker_build
 
-        image = dockerbuild.Image("image",
-            cache_from=[dockerbuild.CacheFromArgs(
-                local=dockerbuild.CacheFromLocalArgs(
+        image = docker_build.Image("image",
+            cache_from=[docker_build.CacheFromArgs(
+                local=docker_build.CacheFromLocalArgs(
                     src="tmp/cache",
                 ),
             )],
-            cache_to=[dockerbuild.CacheToArgs(
-                local=dockerbuild.CacheToLocalArgs(
+            cache_to=[docker_build.CacheToArgs(
+                local=docker_build.CacheToLocalArgs(
                     dest="tmp/cache",
-                    mode=dockerbuild.CacheMode.MAX,
+                    mode=docker_build.CacheMode.MAX,
                 ),
             )],
-            context=dockerbuild.BuildContextArgs(
+            context=docker_build.BuildContextArgs(
                 location="app",
-            ))
+            ),
+            push=False)
         ```
         ### Docker Build Cloud
         ```python
         import pulumi
-        import pulumi_dockerbuild as dockerbuild
+        import pulumi_docker_build as docker_build
 
-        image = dockerbuild.Image("image",
-            builder=dockerbuild.BuilderConfigArgs(
+        image = docker_build.Image("image",
+            builder=docker_build.BuilderConfigArgs(
                 name="cloud-builder-name",
             ),
-            context=dockerbuild.BuildContextArgs(
+            context=docker_build.BuildContextArgs(
                 location="app",
             ),
-            exec_=True)
+            exec_=True,
+            push=False)
         ```
         ### Build arguments
         ```python
         import pulumi
-        import pulumi_dockerbuild as dockerbuild
+        import pulumi_docker_build as docker_build
 
-        image = dockerbuild.Image("image",
+        image = docker_build.Image("image",
             build_args={
                 "SET_ME_TO_TRUE": "true",
             },
-            context=dockerbuild.BuildContextArgs(
+            context=docker_build.BuildContextArgs(
                 location="app",
-            ))
+            ),
+            push=False)
         ```
         ### Build target
         ```python
         import pulumi
-        import pulumi_dockerbuild as dockerbuild
+        import pulumi_docker_build as docker_build
 
-        image = dockerbuild.Image("image",
-            context=dockerbuild.BuildContextArgs(
+        image = docker_build.Image("image",
+            context=docker_build.BuildContextArgs(
                 location="app",
             ),
+            push=False,
             target="build-me")
         ```
         ### Named contexts
         ```python
         import pulumi
-        import pulumi_dockerbuild as dockerbuild
+        import pulumi_docker_build as docker_build
 
-        image = dockerbuild.Image("image", context=dockerbuild.BuildContextArgs(
-            location="app",
-            named={
-                "golang:latest": dockerbuild.ContextArgs(
-                    location="docker-image://golang@sha256:b8e62cf593cdaff36efd90aa3a37de268e6781a2e68c6610940c48f7cdf36984",
-                ),
-            },
-        ))
+        image = docker_build.Image("image",
+            context=docker_build.BuildContextArgs(
+                location="app",
+                named={
+                    "golang:latest": docker_build.ContextArgs(
+                        location="docker-image://golang@sha256:b8e62cf593cdaff36efd90aa3a37de268e6781a2e68c6610940c48f7cdf36984",
+                    ),
+                },
+            ),
+            push=False)
         ```
         ### Remote context
         ```python
         import pulumi
-        import pulumi_dockerbuild as dockerbuild
+        import pulumi_docker_build as docker_build
 
-        image = dockerbuild.Image("image", context=dockerbuild.BuildContextArgs(
-            location="https://raw.githubusercontent.com/pulumi/pulumi-docker/api-types/provider/testdata/Dockerfile",
-        ))
+        image = docker_build.Image("image",
+            context=docker_build.BuildContextArgs(
+                location="https://raw.githubusercontent.com/pulumi/pulumi-docker/api-types/provider/testdata/Dockerfile",
+            ),
+            push=False)
         ```
         ### Inline Dockerfile
         ```python
         import pulumi
-        import pulumi_dockerbuild as dockerbuild
+        import pulumi_docker_build as docker_build
 
-        image = dockerbuild.Image("image",
-            context=dockerbuild.BuildContextArgs(
+        image = docker_build.Image("image",
+            context=docker_build.BuildContextArgs(
                 location="app",
             ),
-            dockerfile=dockerbuild.DockerfileArgs(
+            dockerfile=docker_build.DockerfileArgs(
                 inline=\"\"\"FROM busybox
         COPY hello.c ./
         \"\"\",
-            ))
+            ),
+            push=False)
         ```
         ### Remote context
         ```python
         import pulumi
-        import pulumi_dockerbuild as dockerbuild
+        import pulumi_docker_build as docker_build
 
-        image = dockerbuild.Image("image",
-            context=dockerbuild.BuildContextArgs(
+        image = docker_build.Image("image",
+            context=docker_build.BuildContextArgs(
                 location="https://github.com/docker-library/hello-world.git",
             ),
-            dockerfile=dockerbuild.DockerfileArgs(
+            dockerfile=docker_build.DockerfileArgs(
                 location="app/Dockerfile",
-            ))
+            ),
+            push=False)
         ```
         ### Local export
         ```python
         import pulumi
-        import pulumi_dockerbuild as dockerbuild
+        import pulumi_docker_build as docker_build
 
-        image = dockerbuild.Image("image",
-            context=dockerbuild.BuildContextArgs(
+        image = docker_build.Image("image",
+            context=docker_build.BuildContextArgs(
                 location="app",
             ),
-            exports=[dockerbuild.ExportArgs(
-                docker=dockerbuild.ExportDockerArgs(
+            exports=[docker_build.ExportArgs(
+                docker=docker_build.ExportDockerArgs(
                     tar=True,
                 ),
-            )])
+            )],
+            push=False)
         ```
 
         :param str resource_name: The name of the resource.
         :param ImageArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
@@ -1394,14 +1394,16 @@
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ImageArgs.__new__(ImageArgs)
 
             __props__.__dict__["add_hosts"] = add_hosts
             __props__.__dict__["build_args"] = build_args
+            if build_on_preview is None:
+                build_on_preview = True
             __props__.__dict__["build_on_preview"] = build_on_preview
             __props__.__dict__["builder"] = builder
             __props__.__dict__["cache_from"] = cache_from
             __props__.__dict__["cache_to"] = cache_to
             __props__.__dict__["context"] = context
             __props__.__dict__["dockerfile"] = dockerfile
             __props__.__dict__["exec_"] = exec_
@@ -1410,14 +1412,16 @@
             __props__.__dict__["load"] = load
             if network is None:
                 network = 'default'
             __props__.__dict__["network"] = network
             __props__.__dict__["no_cache"] = no_cache
             __props__.__dict__["platforms"] = platforms
             __props__.__dict__["pull"] = pull
+            if push is None and not opts.urn:
+                raise TypeError("Missing required property 'push'")
             __props__.__dict__["push"] = push
             __props__.__dict__["registries"] = registries
             __props__.__dict__["secrets"] = secrets
             __props__.__dict__["ssh"] = ssh
             __props__.__dict__["tags"] = tags
             __props__.__dict__["target"] = target
             __props__.__dict__["context_hash"] = None
@@ -1498,28 +1502,25 @@
         """
         return pulumi.get(self, "build_args")
 
     @property
     @pulumi.getter(name="buildOnPreview")
     def build_on_preview(self) -> pulumi.Output[Optional[bool]]:
         """
-        By default, preview behavior depends on the execution environment. If
-        Pulumi detects the operation is running on a CI system (GitHub Actions,
-        Travis CI, Azure Pipelines, etc.) then it will build images during
-        previews as a safeguard. Otherwise, if not running on CI, previews will
-        not build images.
-
-        Setting this to `false` forces previews to never perform builds, and
-        setting it to `true` will always build the image during previews.
+        Setting this to `false` will always skip image builds during previews,
+        and setting it to `true` will always build images during previews.
 
         Images built during previews are never exported to registries, however
         cache manifests are still exported.
 
         On-disk Dockerfiles are always validated for syntactic correctness
         regardless of this setting.
+
+        Defaults to `true` as a safeguard against broken images merging as part
+        of CI pipelines.
         """
         return pulumi.get(self, "build_on_preview")
 
     @property
     @pulumi.getter
     def builder(self) -> pulumi.Output[Optional['outputs.BuilderConfig']]:
         """
@@ -1696,15 +1697,15 @@
 
         Equivalent to Docker's `--pull` flag.
         """
         return pulumi.get(self, "pull")
 
     @property
     @pulumi.getter
-    def push(self) -> pulumi.Output[Optional[bool]]:
+    def push(self) -> pulumi.Output[bool]:
         """
         When `true` the build will automatically include a `registry` export.
 
         Defaults to `false`.
 
         Equivalent to Docker's `--push` flag.
         """
```

### Comparing `pulumi_docker_build-0.0.1a3/pulumi_docker_build/index.py` & `pulumi_docker_build-0.0.2/pulumi_docker_build/index.py`

 * *Files 9% similar despite different names*

```diff
@@ -100,21 +100,33 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  push: Optional[pulumi.Input[bool]] = None,
                  registry: Optional[pulumi.Input[pulumi.InputType['RegistryArgs']]] = None,
                  sources: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tag: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        An index (or manifest list) referencing one or more existing images.
+        A wrapper around `docker buildx imagetools create` to create an index
+        (or manifest list) referencing one or more existing images.
 
-        Useful for crafting a multi-platform image from several
-        platform-specific images.
+        In most cases you do not need an `Index` to build a multi-platform
+        image -- specifying multiple platforms on the `Image` will handle this
+        for you automatically.
+
+        However, as of April 2024, building multi-platform images _with
+        caching_ will only export a cache for one platform at a time (see [this
+        discussion](https://github.com/docker/buildx/discussions/1382) for more
+        details).
+
+        Therefore this resource can be helpful if you are building
+        multi-platform images with caching: each platform can be built and
+        cached separately, and an `Index` can join them all together. An
+        example of this is shown below.
 
-        This creates an OCI image index or a Docker manifest list depending on
-        the media types of the source images.
+        This resource creates an OCI image index or a Docker manifest list
+        depending on the media types of the source images.
 
         ## Example Usage
         ### Multi-platform registry caching
         ```python
         import pulumi
         import pulumi_docker_build as docker_build
 
@@ -175,21 +187,33 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: IndexArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        An index (or manifest list) referencing one or more existing images.
+        A wrapper around `docker buildx imagetools create` to create an index
+        (or manifest list) referencing one or more existing images.
 
-        Useful for crafting a multi-platform image from several
-        platform-specific images.
+        In most cases you do not need an `Index` to build a multi-platform
+        image -- specifying multiple platforms on the `Image` will handle this
+        for you automatically.
+
+        However, as of April 2024, building multi-platform images _with
+        caching_ will only export a cache for one platform at a time (see [this
+        discussion](https://github.com/docker/buildx/discussions/1382) for more
+        details).
+
+        Therefore this resource can be helpful if you are building
+        multi-platform images with caching: each platform can be built and
+        cached separately, and an `Index` can join them all together. An
+        example of this is shown below.
 
-        This creates an OCI image index or a Docker manifest list depending on
-        the media types of the source images.
+        This resource creates an OCI image index or a Docker manifest list
+        depending on the media types of the source images.
 
         ## Example Usage
         ### Multi-platform registry caching
         ```python
         import pulumi
         import pulumi_docker_build as docker_build
```

### Comparing `pulumi_docker_build-0.0.1a3/pulumi_docker_build/outputs.py` & `pulumi_docker_build-0.0.2/pulumi_docker_build/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.0.1a3/pulumi_docker_build/provider.py` & `pulumi_docker_build-0.0.2/pulumi_docker_build/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.0.1a3/pulumi_docker_build.egg-info/SOURCES.txt` & `pulumi_docker_build-0.0.2/pulumi_docker_build.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_docker_build-0.0.1a3/pyproject.toml` & `pulumi_docker_build-0.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
   name = "pulumi_docker_build"
-  description = "A Pulumi provider for Docker buildx"
+  description = "A Pulumi provider for building modern Docker images with buildx and BuildKit."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
-  keywords = ["docker", "buildkit", "buildx"]
+  keywords = ["docker", "buildkit", "buildx", "kind/native"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.1a3"
+  version = "0.0.2"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
-    Homepage = "https://pulumi.io"
+    Homepage = "https://pulumi.com"
     Repository = "https://github.com/pulumi/pulumi-docker-build"
 
 [build-system]
   requires = ["setuptools>=61.0"]
   build-backend = "setuptools.build_meta"
 
 [tool]
```

