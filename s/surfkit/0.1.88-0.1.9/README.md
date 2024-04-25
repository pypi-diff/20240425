# Comparing `tmp/surfkit-0.1.88.tar.gz` & `tmp/surfkit-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surfkit-0.1.88.tar", max compression
+gzip compressed data, was "surfkit-0.1.9.tar", max compression
```

## Comparing `surfkit-0.1.88.tar` & `surfkit-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,13 @@
--rw-r--r--   0        0        0     1069 2024-04-09 16:39:37.152115 surfkit-0.1.88/LICENSE
--rw-r--r--   0        0        0      270 2024-04-03 02:13:16.594885 surfkit-0.1.88/README.md
--rw-r--r--   0        0        0      697 2024-04-25 16:57:36.707170 surfkit-0.1.88/pyproject.toml
--rw-r--r--   0        0        0     1726 2024-04-11 17:52:32.512640 surfkit-0.1.88/surfkit/agent.py
--rw-r--r--   0        0        0      602 2024-04-09 16:39:37.166082 surfkit-0.1.88/surfkit/cli/init.py
--rw-r--r--   0        0        0     6629 2024-04-17 22:08:07.372842 surfkit-0.1.88/surfkit/cli/main.py
--rw-r--r--   0        0        0    10733 2024-04-16 17:55:09.920080 surfkit-0.1.88/surfkit/cli/templates/agent.py
--rw-r--r--   0        0        0        0 2024-04-09 16:39:37.166494 surfkit-0.1.88/surfkit/cli/templates/device.py
--rw-r--r--   0        0        0     2053 2024-04-17 19:36:14.985684 surfkit-0.1.88/surfkit/config.py
--rw-r--r--   0        0        0     2007 2024-04-17 19:23:41.286231 surfkit-0.1.88/surfkit/db/conn.py
--rw-r--r--   0        0        0      982 2024-04-17 16:29:32.098357 surfkit-0.1.88/surfkit/db/models.py
--rw-r--r--   0        0        0      238 2024-04-17 19:35:04.174976 surfkit-0.1.88/surfkit/env.py
--rw-r--r--   0        0        0      993 2024-04-03 16:40:15.124046 surfkit-0.1.88/surfkit/hub.py
--rw-r--r--   0        0        0     7553 2024-04-17 00:47:37.183302 surfkit-0.1.88/surfkit/llm.py
--rw-r--r--   0        0        0     2413 2024-04-17 16:28:56.465927 surfkit-0.1.88/surfkit/models.py
--rw-r--r--   0        0        0     3027 2024-04-19 03:18:18.336114 surfkit-0.1.88/surfkit/runtime/agent/base.py
--rw-r--r--   0        0        0     7374 2024-04-19 03:20:01.944064 surfkit-0.1.88/surfkit/runtime/agent/docker.py
--rw-r--r--   0        0        0    27123 2024-04-19 03:19:51.631082 surfkit-0.1.88/surfkit/runtime/agent/kube.py
--rw-r--r--   0        0        0      910 2024-04-19 03:20:06.559203 surfkit-0.1.88/surfkit/runtime/agent/load.py
--rw-r--r--   0        0        0     1425 2024-04-11 22:52:18.482166 surfkit-0.1.88/surfkit/runtime/container/base.py
--rw-r--r--   0        0        0     5983 2024-04-16 16:34:59.842004 surfkit-0.1.88/surfkit/runtime/container/docker.py
--rw-r--r--   0        0        0    16077 2024-04-11 22:50:31.352813 surfkit-0.1.88/surfkit/runtime/container/kube.py
--rw-r--r--   0        0        0     1028 2024-04-11 16:49:49.850218 surfkit-0.1.88/surfkit/runtime/container/load.py
--rw-r--r--   0        0        0      402 2024-04-11 18:32:09.170609 surfkit-0.1.88/surfkit/runtime/vm/base.py
--rw-r--r--   0        0        0     9920 2024-04-17 20:04:44.519945 surfkit-0.1.88/surfkit/types.py
--rw-r--r--   0        0        0     1221 1970-01-01 00:00:00.000000 surfkit-0.1.88/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-02 20:08:38.101639 surfkit-0.1.9/LICENSE
+-rw-r--r--   0        0        0      270 2024-04-03 02:13:16.594885 surfkit-0.1.9/README.md
+-rw-r--r--   0        0        0      442 2024-04-04 18:10:08.442909 surfkit-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      610 2024-04-03 16:41:37.648579 surfkit-0.1.9/surfkit/agent.py
+-rw-r--r--   0        0        0        0 2024-04-03 16:41:36.393225 surfkit-0.1.9/surfkit/cli.py
+-rw-r--r--   0        0        0     2013 2024-04-03 02:11:06.207281 surfkit-0.1.9/surfkit/db/conn.py
+-rw-r--r--   0        0        0     1473 2024-04-03 16:41:49.842770 surfkit-0.1.9/surfkit/db/models.py
+-rw-r--r--   0        0        0      195 2024-04-03 16:41:34.576256 surfkit-0.1.9/surfkit/env.py
+-rw-r--r--   0        0        0      993 2024-04-03 16:40:15.124046 surfkit-0.1.9/surfkit/hub.py
+-rw-r--r--   0        0        0     5562 2024-04-03 22:24:56.115885 surfkit-0.1.9/surfkit/llm.py
+-rw-r--r--   0        0        0     1721 2024-04-03 20:39:21.080498 surfkit-0.1.9/surfkit/models.py
+-rw-r--r--   0        0        0     9000 2024-04-03 02:10:58.047265 surfkit-0.1.9/surfkit/types.py
+-rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 surfkit-0.1.9/PKG-INFO
```

### Comparing `surfkit-0.1.88/surfkit/db/conn.py` & `surfkit-0.1.9/surfkit/db/conn.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,17 +33,17 @@
         client_encoding="utf8",
     )
 
     return engine
 
 
 def get_sqlite_conn() -> Engine:
-    print("\nconnecting to local sqlite db ./data/surfkit.db")
-    os.makedirs(os.path.dirname("./data/surfkit.db"), exist_ok=True)
-    engine = create_engine("sqlite:///./data/surfkit.db")
+    print("\nconnecting to local sqlite db ./data/guisurfer.db")
+    os.makedirs(os.path.dirname("./data/guisurfer.db"), exist_ok=True)
+    engine = create_engine("sqlite:///./data/guisurfer.db")
     return engine
 
 
 if DB_TYPE == "postgres":
     engine = get_pg_conn()
 else:
     engine = get_sqlite_conn()
```

### Comparing `surfkit-0.1.88/surfkit/db/models.py` & `surfkit-0.1.9/surfkit/db/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,52 @@
 import uuid
 import time
 
 from sqlalchemy import Column, String, Boolean, Float, Integer
 from sqlalchemy.orm import declarative_base
 
+from ..models import V1UserProfile
 
 Base = declarative_base()
 
 
+class UserRecord(Base):
+    __tablename__ = "users"
+
+    email = Column(String, unique=True, index=True, primary_key=True)
+    display_name = Column(String)
+    handle = Column(String)
+    picture = Column(String)
+    created = Column(Integer)
+    updated = Column(Integer)
+
+    def to_v1_schema(self) -> V1UserProfile:
+        return V1UserProfile(
+            email=self.email,
+            display_name=self.display_name,
+            picture=self.picture,
+            created=self.created,
+            updated=self.updated,
+        )
+
+
 class AgentTypeRecord(Base):
     __tablename__ = "agent_types"
 
     id = Column(String, primary_key=True, default=lambda: str(uuid.uuid4()))
     name = Column(String, unique=True, index=True)
     description = Column(String)
     image = Column(String)
-    versions = Column(String, nullable=True)
-    repo = Column(String, nullable=True)
+    versions = Column(String)
     env_opts = Column(String)
-    runtimes = Column(String)
+    supported_runtimes = Column(String)
     owner_id = Column(String)
     public = Column(Boolean)
     icon = Column(String)
     created = Column(Float, default=time.time)
     updated = Column(Float, default=time.time)
-    resource_requests = Column(String, nullable=True)
-    resource_limits = Column(String, nullable=True)
+    mem_request = Column(String)
+    mem_limit = Column(String)
+    cpu_request = Column(String)
+    cpu_limit = Column(String)
+    gpu_mem = Column(String)
     llm_providers = Column(String, nullable=True)
-    devices = Column(String, nullable=True)
-    meters = Column(String, nullable=True)
```

### Comparing `surfkit-0.1.88/surfkit/hub.py` & `surfkit-0.1.9/surfkit/hub.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.88/surfkit/models.py` & `surfkit-0.1.9/surfkit/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,90 +12,55 @@
     options: List[str] = []
 
 
 class LLMProviders(BaseModel):
     preference: List[str] = []
 
 
-class DeviceConfig(BaseModel):
-    name: str
-    provision: bool = False
-
-
-class DevicesConfig(BaseModel):
-    preference: List[DeviceConfig] = []
-
-
 class LLMProviderOption(BaseModel):
     model: str
     env_var: EnvVarOptModel
 
 
 class LLMProviderModel(BaseModel):
     options: List[LLMProviderOption]
 
 
-class MeterModel(BaseModel):
-    name: str
-    unit: str
-    cost: float
-    description: Optional[str] = None
-
-
-class RuntimeModel(BaseModel):
-    type: str
-    preference: List[str] = []
-
-
-class ResourceLimitsModel(BaseModel):
-    cpu: str = "2"
-    memory: str = "2Gi"
-
-
-class ResourceRequestsModel(BaseModel):
-    cpu: str = "1"
-    memory: str = "500m"
-    gpu: Optional[str] = None
-
-
 class AgentTypeModel(BaseModel):
-    version: Optional[str] = None
-    kind: Optional[str] = None
     id: Optional[str] = None
     name: str
-    description: str
     owner_id: Optional[str] = None
-    repo: Optional[str] = None
+    description: str
     image: Optional[str] = None
     versions: Optional[Dict[str, str]] = None
     env_opts: List[EnvVarOptModel] = []
-    runtimes: List[RuntimeModel] = []
+    supported_runtimes: List[str] = []
     created: Optional[float] = None
     updated: Optional[float] = None
     public: bool = False
     icon: Optional[str] = None
-    resource_requests: ResourceRequestsModel = ResourceRequestsModel()
-    resource_limits: ResourceLimitsModel = ResourceLimitsModel()
+    mem_request: Optional[str] = "500m"
+    mem_limit: Optional[str] = "2gi"
+    cpu_request: Optional[str] = "1"
+    cpu_limit: Optional[str] = "4"
+    gpu_mem: Optional[str] = None
     llm_providers: Optional[LLMProviders] = None
-    devices: List[DeviceConfig] = []
-    meters: List[MeterModel] = []
 
 
 class AgentTypesModel(BaseModel):
     types: List[AgentTypeModel]
 
 
 class CreateAgentTypeModel(BaseModel):
     id: str
     name: str
     description: str
     image: str
     env_opts: List[EnvVarOptModel] = []
     supported_runtimes: List[str] = []
-    versions: Dict[str, str] = {}
     public: bool = False
     icon: Optional[str] = None
 
 
 class V1UserProfile(BaseModel):
     email: Optional[str] = None
     display_name: Optional[str] = None
```

### Comparing `surfkit-0.1.88/surfkit/types.py` & `surfkit-0.1.9/surfkit/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,257 +1,225 @@
 from typing import List, Optional, Dict
 import uuid
 import time
 import json
 
-from sqlalchemy import or_
+from sqlalchemy import or_, and_
 
 from .db.models import AgentTypeRecord
 from .db.conn import WithDB
 from .models import (
     EnvVarOptModel,
     AgentTypeModel,
     LLMProviders,
-    LLMProviders,
-    DeviceConfig,
-    RuntimeModel,
-    MeterModel,
-    ResourceLimitsModel,
-    ResourceRequestsModel,
 )
 
+from .models import LLMProviders
+
 
 class AgentType(WithDB):
     """A type of agent"""
 
     def __init__(
         self,
         name: str,
         description: str,
         image: str,
         versions: Dict[str, str],
-        runtimes: List[RuntimeModel] = [],
+        supported_runtimes: List[str],
         owner_id: Optional[str] = None,
         env_opts: List[EnvVarOptModel] = [],
         public: bool = False,
         icon: Optional[str] = None,
-        resource_requests: ResourceRequestsModel = ResourceRequestsModel(),
-        resource_limits: ResourceLimitsModel = ResourceLimitsModel(),
+        mem_request: Optional[str] = "500m",
+        mem_limit: Optional[str] = "2gi",
+        cpu_request: Optional[str] = "1",
+        cpu_limit: Optional[str] = "4",
+        gpu_mem: Optional[str] = None,
         llm_providers: Optional[LLMProviders] = None,
-        devices: List[DeviceConfig] = [],
-        repo: Optional[str] = None,
-        meters: List[MeterModel] = [],
     ):
         self.id = str(uuid.uuid4())
         self.name = name
         self.description = description
         self.image = image
         self.versions = versions
-        self.runtimes = runtimes
+        self.supported_runtimes = supported_runtimes
         self.owner_id = owner_id
         self.env_opts = env_opts
         self.public = public
         self.icon = icon
-        self.resource_requests = resource_requests
-        self.resource_limits = resource_limits
+        self.mem_request = mem_request
+        self.mem_limit = mem_limit
+        self.cpu_request = cpu_request
+        self.cpu_limit = cpu_limit
+        self.gpu_mem = gpu_mem
         self.created = time.time()
         self.updated = time.time()
         self.llm_providers: Optional[LLMProviders] = llm_providers
-        self.devices = devices
-        self.repo = repo
-        self.meters = meters
         self.save()
 
     def to_schema(self) -> AgentTypeModel:
         return AgentTypeModel(
             id=self.id,
             name=self.name,
             description=self.description,
             image=self.image,
             versions=self.versions,
             env_opts=self.env_opts,
-            runtimes=self.runtimes,
+            supported_runtimes=self.supported_runtimes,
             created=self.created,
             updated=self.updated,
             public=self.public,
             icon=self.icon,
-            resource_requests=self.resource_requests,
-            resource_limits=self.resource_limits,
+            mem_request=self.mem_request,
+            mem_limit=self.mem_limit,
+            cpu_request=self.cpu_request,
+            cpu_limit=self.cpu_limit,
+            gpu_mem=self.gpu_mem,
             llm_providers=self.llm_providers,
-            devices=self.devices,
             owner_id=self.owner_id,
-            repo=self.repo,
-            meters=self.meters,
         )
 
     @classmethod
     def from_schema(cls, schema: AgentTypeModel) -> "AgentType":
         obj = cls.__new__(cls)
         obj.id = schema.id
         obj.name = schema.name
         obj.owner_id = schema.owner_id
         obj.description = schema.description
         obj.image = schema.image
         obj.env_opts = schema.env_opts
-        obj.runtimes = schema.runtimes
+        obj.supported_runtimes = schema.supported_runtimes
         obj.created = schema.created
         obj.updated = schema.updated
         obj.public = schema.public
         obj.icon = schema.icon
-        obj.resource_requests = schema.resource_requests
-        obj.resource_limits = schema.resource_limits
+        obj.mem_limit = schema.mem_limit
+        obj.mem_request = schema.mem_request
+        obj.cpu_limit = schema.cpu_limit
+        obj.cpu_request = schema.cpu_request
+        obj.gpu_mem = schema.gpu_mem
         obj.versions = schema.versions
         obj.llm_providers = schema.llm_providers
-        obj.devices = schema.devices
-        obj.repo = schema.repo
-        obj.meters = schema.meters
         return obj
 
     def to_record(self) -> AgentTypeRecord:
         versions = json.dumps(self.versions)
         llm_providers = None
         if self.llm_providers:
             llm_providers = json.dumps(self.llm_providers.model_dump())
-
-        meters = None
-        if self.meters:
-            meters = json.dumps([meter.model_dump() for meter in self.meters])
-
-        devices = None
-        if self.devices:
-            devices = json.dumps(self.devices)
         return AgentTypeRecord(
             id=self.id,
             name=self.name,
             description=self.description,
             image=self.image,
             versions=versions,
             env_opts=json.dumps([opt.model_dump() for opt in self.env_opts]),
-            runtimes=json.dumps([runtime.model_dump() for runtime in self.runtimes]),
+            supported_runtimes=json.dumps(self.supported_runtimes),
             created=self.created,
             updated=self.updated,
             owner_id=self.owner_id,
             public=self.public,
             icon=self.icon,
-            resource_limits=json.dumps(self.resource_limits.model_dump()),
-            resource_requests=json.dumps(self.resource_requests.model_dump()),
+            mem_limit=self.mem_limit,
+            mem_request=self.mem_request,
+            cpu_limit=self.cpu_limit,
+            cpu_request=self.cpu_request,
+            gpu_mem=self.gpu_mem,
             llm_providers=llm_providers,
-            devices=devices,
-            meters=meters,
-            repo=self.repo,
         )
 
     @classmethod
     def from_record(cls, record: AgentTypeRecord) -> "AgentType":
         versions = {}
-        if record.versions:  # type: ignore
-            versions = json.loads(str(record.versions))
-
-        llm_providers = None
-        if record.llm_providers:  # type: ignore
-            llm_providers = LLMProviders(**json.loads(str(record.llm_providers)))
-
-        devices = []
-        if record.devices:  # type: ignore
-            devices = json.loads(str(record.devices))
-
-        meters = []
-        if record.meters:  # type: ignore
-            meters_mod = json.loads(str(record.meters))
-            meters = [MeterModel(**m) for m in meters_mod]
-
+        if record.versions:
+            versions = json.loads(record.versions)
+        if record.llm_providers:
+            llm_providers = LLMProviders(**json.loads(record.llm_providers))
         obj = cls.__new__(cls)
         obj.id = record.id
         obj.name = record.name
         obj.description = record.description
         obj.image = record.image
         obj.versions = versions
-        obj.env_opts = [
-            EnvVarOptModel(**opt) for opt in json.loads(str(record.env_opts))
-        ]
-        obj.runtimes = [
-            RuntimeModel(**runtime) for runtime in json.loads(str(record.runtimes))
-        ]
+        obj.env_opts = [EnvVarOptModel(**opt) for opt in json.loads(record.env_opts)]
+        obj.supported_runtimes = json.loads(record.supported_runtimes)
         obj.created = record.created
         obj.updated = record.updated
         obj.owner_id = record.owner_id
         obj.public = record.public
         obj.icon = record.icon
-        obj.resource_requests = (
-            ResourceRequestsModel(**json.loads(str(record.resource_requests)))
-            if record.resource_requests  # type: ignore
-            else ResourceRequestsModel()
-        )
-        obj.resource_limits = (
-            ResourceLimitsModel(**json.loads(str(record.resource_limits)))
-            if record.resource_limits  # type: ignore
-            else ResourceLimitsModel()
-        )
+        obj.mem_limit = record.mem_limit
+        obj.mem_request = record.mem_request
+        obj.cpu_limit = record.cpu_limit
+        obj.cpu_request = record.cpu_request
+        obj.gpu_mem = record.gpu_mem
         obj.llm_providers = llm_providers
-        obj.devices = devices
-        obj.meters = meters
-        obj.repo = record.repo
         return obj
 
     def save(self) -> None:
         for session in self.get_db():
             if session:
                 record = self.to_record()
                 session.merge(record)
                 session.commit()
 
     @classmethod
     def find(cls, **kwargs) -> List["AgentType"]:
         for session in cls.get_db():
-            records = session.query(AgentTypeRecord).filter_by(**kwargs).all()
-            return [cls.from_record(record) for record in records]
-
-        return []
+            if session:
+                records = session.query(AgentTypeRecord).filter_by(**kwargs).all()
+                return [cls.from_record(record) for record in records]
 
     @classmethod
     def find_for_user(
         cls, user_id: str, name: Optional[str] = None
     ) -> List["AgentType"]:
         for session in cls.get_db():
-            # Base query
-            query = session.query(AgentTypeRecord).filter(
-                or_(
-                    AgentTypeRecord.owner_id == user_id,  # type: ignore
-                    AgentTypeRecord.public == True,
+            if session:
+                # Base query
+                query = session.query(AgentTypeRecord).filter(
+                    or_(
+                        AgentTypeRecord.owner_id == user_id,
+                        AgentTypeRecord.public == True,
+                    )
                 )
-            )
 
-            # Conditionally add name filter if name is provided
-            if name is not None:
-                query = query.filter(AgentTypeRecord.name == name)
-
-            records = query.all()
-            return [cls.from_record(record) for record in records]
-        return []
+                # Conditionally add name filter if name is provided
+                if name is not None:
+                    query = query.filter(AgentTypeRecord.name == name)
+
+                records = query.all()
+                return [cls.from_record(record) for record in records]
 
     @classmethod
-    def delete(cls, name: str, owner_id: str) -> None:
+    def delete(cls, id: str, owner_id: str) -> None:
         for session in cls.get_db():
             if session:
                 record = (
                     session.query(AgentTypeRecord)
-                    .filter_by(name=name, owner_id=owner_id)
+                    .filter_by(id=id, owner_id=owner_id)
                     .first()
                 )
                 if record:
                     session.delete(record)
                     session.commit()
 
     def update(self, model: AgentTypeModel) -> None:
         """
         Updates the current AgentType instance with values from an AgentTypeModel instance.
         """
         # Track if any updates are needed
         updated = False
 
+        # Compare and update fields
+        if self.name != model.name:
+            self.name = model.name
+            updated = True
+
         if self.description != model.description:
             self.description = model.description
             updated = True
 
         if self.image != model.image:
             self.image = model.image
             updated = True
@@ -260,47 +228,47 @@
             self.versions = model.versions
             updated = True
 
         if self.env_opts != model.env_opts:
             self.env_opts = model.env_opts
             updated = True
 
-        if self.runtimes != model.runtimes:
-            self.runtimes = model.runtimes
+        if self.supported_runtimes != model.supported_runtimes:
+            self.supported_runtimes = model.supported_runtimes
             updated = True
 
         if self.public != model.public:
             self.public = model.public
             updated = True
 
         if self.icon != model.icon:
             self.icon = model.icon
             updated = True
 
-        if self.resource_requests != model.resource_requests:
-            self.resource_requests = model.resource_requests
+        if self.mem_request != model.mem_request:
+            self.mem_request = model.mem_request
             updated = True
 
-        if self.resource_limits != model.resource_limits:
-            self.resource_limits = model.resource_limits
+        if self.mem_limit != model.mem_limit:
+            self.mem_limit = model.mem_limit
             updated = True
 
-        if self.llm_providers != model.llm_providers:
-            self.llm_providers = model.llm_providers
+        if self.cpu_request != model.cpu_request:
+            self.cpu_request = model.cpu_request
             updated = True
 
-        if self.devices != model.devices:
-            self.devices = model.devices
+        if self.cpu_limit != model.cpu_limit:
+            self.cpu_limit = model.cpu_limit
             updated = True
 
-        if self.meters != model.meters:
-            self.meters = model.meters
+        if self.gpu_mem != model.gpu_mem:
+            self.gpu_mem = model.gpu_mem
             updated = True
 
-        if self.repo != model.repo:
-            self.repo = model.repo
+        if self.llm_providers != model.llm_providers:
+            self.llm_providers = model.llm_providers
             updated = True
 
         # If anything was updated, set the updated timestamp and save changes
         if updated:
             self.updated = time.time()
             self.save()
```

