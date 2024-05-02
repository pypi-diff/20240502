# Comparing `tmp/poaster-1.3.0.tar.gz` & `tmp/poaster-1.4.0.tar.gz`

## Comparing `poaster-1.3.0.tar` & `poaster-1.4.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 poaster-1.3.0/.build.yml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 poaster-1.3.0/.envrc
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 poaster-1.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 poaster-1.3.0/scripts/load-fixtures.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/__init__.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/app.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/cli.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/dependencies.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/access/__init__.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/access/api.py
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/access/cli.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/access/components.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/access/repository.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/access/schemas.py
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/access/services.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/access/tables.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/access/web.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/bulletin/__init__.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/bulletin/api.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/bulletin/components.py
--rw-r--r--   0        0        0     6333 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/bulletin/repository.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/bulletin/schemas.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/bulletin/services.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/bulletin/tables.py
--rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/bulletin/web.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/core/__init__.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/core/components.py
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/core/config.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/core/exceptions.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/core/hashing.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/core/http_exceptions.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/core/oauth.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/core/schemas.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/core/sessions.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/core/tables.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/migrations/__init__.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/migrations/alembic.ini
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/migrations/env.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/migrations/script.py.mako
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/migrations/upgrade.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/migrations/versions/0b3ee652b174_.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/migrations/versions/34b9b6b1c9a3_.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/migrations/versions/821b409e627c_.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/static/app.css
--rw-r--r--   0        0        0     6623 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/static/concrete.css
--rw-r--r--   0        0        0     6142 2020-02-02 00:00:00.000000 poaster-1.3.0/src/poaster/static/normalize.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 poaster-1.3.0/tests/__init__.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 poaster-1.3.0/tests/conftest.py
--rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 poaster-1.3.0/tests/test_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 poaster-1.3.0/tests/access/__init__.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 poaster-1.3.0/tests/access/test_api.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 poaster-1.3.0/tests/access/test_cli.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 poaster-1.3.0/tests/access/test_repository.py
--rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 poaster-1.3.0/tests/access/test_services.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 poaster-1.3.0/tests/bulletin/__init__.py
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 poaster-1.3.0/tests/bulletin/test_api.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 poaster-1.3.0/tests/bulletin/test_components.py
--rw-r--r--   0        0        0    10914 2020-02-02 00:00:00.000000 poaster-1.3.0/tests/bulletin/test_repository.py
--rw-r--r--   0        0        0     5511 2020-02-02 00:00:00.000000 poaster-1.3.0/tests/bulletin/test_services.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 poaster-1.3.0/tests/core/__init__.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 poaster-1.3.0/tests/core/test_config.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 poaster-1.3.0/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 poaster-1.3.0/LICENSE
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 poaster-1.3.0/README.md
--rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 poaster-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     3362 2020-02-02 00:00:00.000000 poaster-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 poaster-1.4.0/.build.yml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 poaster-1.4.0/.envrc
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 poaster-1.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 poaster-1.4.0/.nvim/nvim-dap.lua
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 poaster-1.4.0/scripts/load-fixtures.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/__init__.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/app.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/cli.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/dependencies.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/access/__init__.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/access/api.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/access/cli.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/access/components.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/access/repository.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/access/schemas.py
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/access/services.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/access/tables.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/access/web.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/bulletin/__init__.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/bulletin/api.py
+-rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/bulletin/components.py
+-rw-r--r--   0        0        0     6333 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/bulletin/repository.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/bulletin/schemas.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/bulletin/services.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/bulletin/tables.py
+-rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/bulletin/web.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/core/__init__.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/core/components.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/core/config.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/core/exceptions.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/core/hashing.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/core/http_exceptions.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/core/oauth.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/core/schemas.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/core/sessions.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/core/tables.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/migrations/__init__.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/migrations/alembic.ini
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/migrations/env.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/migrations/script.py.mako
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/migrations/upgrade.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/migrations/versions/0b3ee652b174_.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/migrations/versions/34b9b6b1c9a3_.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/migrations/versions/821b409e627c_.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/static/app.css
+-rw-r--r--   0        0        0     6623 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/static/concrete.css
+-rw-r--r--   0        0        0     6142 2020-02-02 00:00:00.000000 poaster-1.4.0/src/poaster/static/normalize.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 poaster-1.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 poaster-1.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 poaster-1.4.0/tests/test_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 poaster-1.4.0/tests/access/__init__.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 poaster-1.4.0/tests/access/test_api.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 poaster-1.4.0/tests/access/test_cli.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 poaster-1.4.0/tests/access/test_repository.py
+-rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 poaster-1.4.0/tests/access/test_services.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 poaster-1.4.0/tests/bulletin/__init__.py
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 poaster-1.4.0/tests/bulletin/test_api.py
+-rw-r--r--   0        0        0    10914 2020-02-02 00:00:00.000000 poaster-1.4.0/tests/bulletin/test_repository.py
+-rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 poaster-1.4.0/tests/bulletin/test_services.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 poaster-1.4.0/tests/core/__init__.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 poaster-1.4.0/tests/core/test_config.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 poaster-1.4.0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 poaster-1.4.0/LICENSE
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 poaster-1.4.0/README.md
+-rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 poaster-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 poaster-1.4.0/PKG-INFO
```

### Comparing `poaster-1.3.0/scripts/load-fixtures.py` & `poaster-1.4.0/scripts/load-fixtures.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,45 +9,33 @@
 import poaster.bulletin.services
 from poaster.core import exceptions, sessions
 
 
 async def load_fixtures():
     """Load test fixtures useful for local development."""
     async with sessions.async_session() as session:
-        u_repo = poaster.access.repository.SqlalchemyUserRepository(session)
-        p_repo = poaster.bulletin.repository.SqlalchemyPostRepository(session)
-        pv_repo = poaster.bulletin.repository.SqlalchemyPostVersionRepository(session)
+        access_svc = poaster.access.services.AccessService.from_session(session)
+        bulletin_svc = poaster.bulletin.services.BulletinService.from_session(session)
 
-        await add_dummy_user(u_repo)
-        await add_dummy_posts(p_repo, pv_repo)
+        await add_dummy_user(access_svc)
+        await add_dummy_posts(bulletin_svc)
 
 
-async def add_dummy_user(
-    user_repository: poaster.access.repository.SupportsUserRepository,
-):
+async def add_dummy_user(access_svc: poaster.access.services.AccessService):
     try:
-        await poaster.access.services.register_user(
-            user_repository=user_repository,
-            username="dummy",
-            password="password",
-        )
+        await access_svc.register_user(username="dummy", password="password")
     except exceptions.AlreadyExists:
         logging.info("'dummy' user already exists with password equal to 'password'.")
     else:
         logging.info("Added 'dummy' user with password equal to 'password'.")
 
 
-async def add_dummy_posts(
-    post_repository: poaster.bulletin.repository.SupportsPostRepository,
-    post_version_repository: poaster.bulletin.repository.SupportsPostVersionRepository,
-):
+async def add_dummy_posts(bulletin_svc: poaster.bulletin.services.BulletinService):
     async def add_post(title: str, text: str):
-        await poaster.bulletin.services.create_post(
-            post_repository,
-            post_version_repository,
+        await bulletin_svc.create_post(
             username="dummy",
             payload=poaster.bulletin.schemas.PostInputSchema(title=title, text=text),
         )
 
     await add_post("Penguins", "Penguins are a group of aquatic flightless birds.")
     await add_post("Tigers", "Tigers are the largest living cat species.")
     await add_post("Koalas", "Koala is is native to Australia.")
```

### Comparing `poaster-1.3.0/src/poaster/app.py` & `poaster-1.4.0/src/poaster/app.py`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/src/poaster/cli.py` & `poaster-1.4.0/src/poaster/cli.py`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/src/poaster/dependencies.py` & `poaster-1.4.0/src/poaster/dependencies.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,34 +24,27 @@
         yield session
         await session.commit()
 
 
 DBSession = Annotated[AsyncSession, Depends(get_db_session)]
 
 
-def get_access_service(
-    db: DBSession,
-) -> poaster.access.services.AccessService:
+def get_access_service(db: DBSession) -> poaster.access.services.AccessService:
     """Instantiate user repository session."""
-    user_repo = poaster.access.repository.SqlalchemyUserRepository(db)
-    return poaster.access.services.AccessService(user_repo)
+    return poaster.access.services.AccessService.from_session(db)
 
 
 AccessService = Annotated[
     poaster.access.services.AccessService, Depends(get_access_service)
 ]
 
 
-def get_bulletin_service(
-    db: DBSession,
-) -> poaster.bulletin.services.BulletinService:
+def get_bulletin_service(db: DBSession) -> poaster.bulletin.services.BulletinService:
     """Instantiate bulletin application service."""
-    post_repo = poaster.bulletin.repository.SqlalchemyPostRepository(db)
-    post_version_repo = poaster.bulletin.repository.SqlalchemyPostVersionRepository(db)
-    return poaster.bulletin.services.BulletinService(post_repo, post_version_repo)
+    return poaster.bulletin.services.BulletinService.from_session(db)
 
 
 BulletinService = Annotated[
     poaster.bulletin.services.BulletinService, Depends(get_bulletin_service)
 ]
```

### Comparing `poaster-1.3.0/src/poaster/access/api.py` & `poaster-1.4.0/src/poaster/access/api.py`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/src/poaster/access/components.py` & `poaster-1.4.0/src/poaster/access/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def login_form() -> H.Element:
     """Login form for authenticating users."""
     return H.fragment(
         H.h1("Login"),
         H.form(action="/login", method="post")(
             H.fieldset(
-                H.legend("Must be logged in to add or edit posts"),
+                H.legend("Log in to add or edit posts"),
                 H.label(for_="username")("Username:"),
                 H.input(type_="text", name="username", required=True),
                 H.label(for_="password")("Password:"),
                 H.input(type_="password", name="password", required=True),
                 H.button(type_="submit")("Login"),
             ),
         ),
```

### Comparing `poaster-1.3.0/src/poaster/access/repository.py` & `poaster-1.4.0/src/poaster/access/repository.py`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/src/poaster/access/schemas.py` & `poaster-1.4.0/src/poaster/access/schemas.py`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/src/poaster/access/services.py` & `poaster-1.4.0/src/poaster/access/services.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,62 @@
+from __future__ import annotations
+
 import dataclasses
 import datetime
 from typing import Optional
 
+from sqlalchemy.ext.asyncio import AsyncSession
+
 from poaster.core import exceptions, hashing, oauth
 
 from . import repository, schemas
 
 
 @dataclasses.dataclass(frozen=True)
 class AccessService:
     """The service layer for the access domain."""
 
-    _user_repository: repository.SupportsUserRepository
+    _user_repo: repository.SupportsUserRepository
+
+    @classmethod
+    def from_session(cls, session: AsyncSession) -> AccessService:
+        """Build access service from database session."""
+        return cls(_user_repo=repository.SqlalchemyUserRepository(session))
 
     async def authenticate(
         self, username: str, password: str
     ) -> Optional[schemas.UserSchema]:
         """Check that input credentials match the user's stored credentials."""
         try:
-            user = await self._user_repository.get_by_username(username)
+            user = await self._user_repo.get_by_username(username)
         except exceptions.DoesNotExist:
             return None
 
         if not hashing.pwd_context.verify(password, user.password):
             return None
 
         return user
 
     async def check_username_exists(self, username: str) -> bool:
         """Check if username exists."""
         try:
-            await self._user_repository.get_by_username(username)
+            await self._user_repo.get_by_username(username)
         except exceptions.DoesNotExist:
             return False
         else:
             return True
 
     async def register_user(self, username: str, password: str) -> schemas.UserSchema:
         """Register user given valid username and password."""
         user = schemas.UserRegistrationSchema(username=username, password=password)
-        return await self._user_repository.create(user)
+        return await self._user_repo.create(user)
 
     async def list_usernames(self) -> list[str]:
         """List out all persisted usernames."""
-        return [user.username for user in await self._user_repository.get_all()]
+        return [user.username for user in await self._user_repo.get_all()]
 
     @classmethod
     def create_access_token(cls, username: str, minutes: int = 60) -> oauth.Token:
         """Generate user access token for a duration of time."""
         payload: oauth.TokenPayload = {
             "sub": username,
             "exp": datetime.datetime.utcnow() + datetime.timedelta(minutes=minutes),
```

### Comparing `poaster-1.3.0/src/poaster/access/web.py` & `poaster-1.4.0/src/poaster/access/web.py`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/src/poaster/bulletin/api.py` & `poaster-1.4.0/src/poaster/bulletin/api.py`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/src/poaster/bulletin/components.py` & `poaster-1.4.0/src/poaster/bulletin/components.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import haitch as H
 
 from poaster.bulletin import schemas, services
-from poaster.core import components, config
+from poaster.core import components
 
 
 def post_form_new() -> H.Element:
     """Form for adding a new post."""
     return H.form(id_="newPost", action="/posts/new", method="post")(
         H.h1("Add new post"),
         H.label(for_="title")("Title:"),
         H.input(id_="title", type_="text", name="title"),
         H.label(for_="text")("Text:"),
-        H.textarea(id_="text", name="text", rows=8),
+        H.textarea(id_="text", name="text", placeholder="Markdown supported", rows=8),
         H.br(),
         H.a(href="/posts", style="padding-right: 1.5rem;")("Back"),
         H.button(type_="submit")("Save"),
     )
 
 
 def post_form_edit(post: schemas.PostSchema) -> H.Element:
@@ -50,32 +50,28 @@
     if not (posts := await bulletin_service.get_posts()):
         return components.message("No posts were found.", variant="warning")
 
     return [
         H.section(
             H.h2(post.title),
             await post_meta_info(bulletin_service, post),
-            post_text_snippet(
-                post.text,
-                max_word_count=config.settings.post_snippet_max_word_count,
-            ),
-            H.a(href=f"/posts/{post.id}")("View"),
+            H.p(H.a(href=f"/posts/{post.id}")("View")),
         )
         for post in posts
     ]
 
 
 async def post_detail(
     bulletin_service: services.BulletinService, post: schemas.PostSchema, username: str
 ) -> H.Element:
     """Detail regarding a post."""
     return H.fragment(
         H.h1(post.title),
         await post_meta_info(bulletin_service, post),
-        H.p(post.text),
+        components.markdown_to_html(post.text),
         H.br(),
         components.links(
             [
                 {
                     "name": "Back",
                     "href": "/posts",
                     "show": True,
@@ -91,20 +87,14 @@
                     "show": username != "",
                 },
             ]
         ),
     )
 
 
-def post_text_snippet(text: str, *, max_word_count: int) -> H.Element:
-    """Text snippet of a post's text."""
-    subset = " ".join(text.split()[: max(max_word_count, 0)])
-    return H.p(text if subset == text else subset + "…")
-
-
 async def post_meta_info(
     bulletin_service: services.BulletinService, post: schemas.PostSchema
 ) -> H.Element:
     """Meta information regarding a post."""
     latest_post = await bulletin_service.get_latest_version_of_post(id=post.id)
     updated_at_str = latest_post.updated_at.strftime("%b %d, %Y at %H:%M")
-    return H.small(f"Last updated on {updated_at_str} UTC")
+    return H.p(H.small(f"Last updated on {updated_at_str} UTC"))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `poaster-1.3.0/src/poaster/bulletin/repository.py` & `poaster-1.4.0/src/poaster/bulletin/repository.py`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/src/poaster/bulletin/schemas.py` & `poaster-1.4.0/src/poaster/bulletin/schemas.py`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/src/poaster/bulletin/tables.py` & `poaster-1.4.0/src/poaster/bulletin/tables.py`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/src/poaster/bulletin/web.py` & `poaster-1.4.0/src/poaster/bulletin/web.py`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/src/poaster/core/components.py` & `poaster-1.4.0/src/poaster/core/components.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Iterable, TypedDict
 
 import haitch as H
+import mistletoe as md
 
 from . import config
 
 
 def page(content: H.SupportsHtml, *, title: str, username: str = "") -> H.Element:
     """Base HTML container for building web pages."""
     return H.html5(
@@ -95,7 +96,14 @@
     style = (
         "padding: 2rem;"
         f"border-left: thick solid {color};"
         f"background: {color}13;"
         "padding-left: 1.2em;"
     )
     return H.p(style=style)(text)
+
+
+def markdown_to_html(text: str) -> H.Element:
+    """Render markdown text to HTML."""
+    with md.HtmlRenderer() as renderer:
+        rendered_html = renderer.render(md.Document(text))
+    return H.unsafe(rendered_html)
```

### Comparing `poaster-1.3.0/src/poaster/core/config.py` & `poaster-1.4.0/src/poaster/core/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     db_path: str = "/./poaster.db"
     secret_key: str = ""
     secret_key_n_bytes: int = 32
     algorithm: str = "HS256"
 
     # theming
     title: str = "poaster"
-    post_snippet_max_word_count: int = 20
     color_danger: str = "#FF595E"
     color_info: str = "#1982C4"
     color_primary: str = "#6A4C93"
     color_success: str = "#8AC926"
     color_warning: str = "#FFCA3A"
 
     @functools.cached_property
```

### Comparing `poaster-1.3.0/src/poaster/core/http_exceptions.py` & `poaster-1.4.0/src/poaster/core/http_exceptions.py`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/src/poaster/core/oauth.py` & `poaster-1.4.0/src/poaster/core/oauth.py`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/src/poaster/core/sessions.py` & `poaster-1.4.0/src/poaster/core/sessions.py`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/src/poaster/migrations/alembic.ini` & `poaster-1.4.0/src/poaster/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/src/poaster/migrations/env.py` & `poaster-1.4.0/src/poaster/migrations/env.py`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/src/poaster/migrations/versions/0b3ee652b174_.py` & `poaster-1.4.0/src/poaster/migrations/versions/0b3ee652b174_.py`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/src/poaster/migrations/versions/34b9b6b1c9a3_.py` & `poaster-1.4.0/src/poaster/migrations/versions/34b9b6b1c9a3_.py`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/src/poaster/migrations/versions/821b409e627c_.py` & `poaster-1.4.0/src/poaster/migrations/versions/821b409e627c_.py`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/src/poaster/static/app.css` & `poaster-1.4.0/src/poaster/static/app.css`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/src/poaster/static/concrete.css` & `poaster-1.4.0/src/poaster/static/concrete.css`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/src/poaster/static/normalize.css` & `poaster-1.4.0/src/poaster/static/normalize.css`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/tests/conftest.py` & `poaster-1.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/tests/test_cli.py` & `poaster-1.4.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/tests/access/test_api.py` & `poaster-1.4.0/tests/access/test_api.py`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/tests/access/test_cli.py` & `poaster-1.4.0/tests/access/test_cli.py`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/tests/access/test_repository.py` & `poaster-1.4.0/tests/access/test_repository.py`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/tests/access/test_services.py` & `poaster-1.4.0/tests/access/test_services.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 import datetime
 
 import pydantic
 import pytest
 from sqlalchemy.ext.asyncio import AsyncSession
 
-from poaster.access import repository, schemas, services
+from poaster.access import schemas, services
 from poaster.core import exceptions, oauth
 
 
 @pytest.fixture
-def user_repo(db_session: AsyncSession) -> repository.SqlalchemyUserRepository:
-    return repository.SqlalchemyUserRepository(db_session)
+def access_service(db_session: AsyncSession) -> services.AccessService:
+    return services.AccessService.from_session(db_session)
 
 
 @pytest.fixture
-async def user(user_repo: repository.SqlalchemyUserRepository) -> schemas.UserSchema:
-    return await user_repo.create(
-        schemas.UserRegistrationSchema(username="bob", password="password")
-    )
-
-
-@pytest.fixture
-def access_service(
-    user_repo: repository.SqlalchemyUserRepository,
-) -> services.AccessService:
-    return services.AccessService(user_repo)
+async def user(access_service: services.AccessService) -> schemas.UserSchema:
+    user = schemas.UserRegistrationSchema(username="bob", password="password")
+    return await access_service._user_repo.create(user)
 
 
 async def test_authenticate_success(
     access_service: services.AccessService, user: schemas.UserSchema
 ):
     got = await access_service.authenticate(user.username, "password")
     want = user
@@ -123,7 +115,13 @@
 async def test_check_username_does_not_exists(access_service: services.AccessService):
     await access_service.register_user("testuser", "password")
 
     got = await access_service.check_username_exists("baduser")
     want = False
 
     assert got == want
+
+
+async def test_duplicate_user_registration(access_service: services.AccessService):
+    await access_service.register_user("testuser", "password")
+    with pytest.raises(exceptions.AlreadyExists):
+        await access_service.register_user("testuser", "password")
```

### Comparing `poaster-1.3.0/tests/bulletin/test_api.py` & `poaster-1.4.0/tests/bulletin/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,9 +125,9 @@
 def test_get_post_not_found(client: TestClient):
     response = client.get("/api/posts/42")
     assert response.status_code == status.HTTP_404_NOT_FOUND
 
 
 @pytest.mark.usefixtures("add_example_posts")
 def test_get_posts(client: TestClient):
-    response = client.get("/api/posts/1")
+    response = client.get("/api/posts")
     assert response.status_code == status.HTTP_200_OK
```

### Comparing `poaster-1.3.0/tests/bulletin/test_repository.py` & `poaster-1.4.0/tests/bulletin/test_repository.py`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/tests/bulletin/test_services.py` & `poaster-1.4.0/tests/bulletin/test_services.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import datetime
 
 import pytest
 from sqlalchemy import text
 from sqlalchemy.ext.asyncio import AsyncSession
 
-from poaster.bulletin import repository, schemas, services
+from poaster.bulletin import schemas, services
 
 
 @pytest.fixture
 def bulletin_service(db_session: AsyncSession) -> services.BulletinService:
-    post_repo = repository.SqlalchemyPostRepository(db_session)
-    post_version_repo = repository.SqlalchemyPostVersionRepository(db_session)
-    return services.BulletinService(post_repo, post_version_repo)
+    return services.BulletinService.from_session(db_session)
 
 
 async def test_create_post(bulletin_service: services.BulletinService):
     got = await bulletin_service.create_post(
         username="testuser",
         payload=schemas.PostInputSchema(title="hi", text="hello, world!"),
     )
```

### Comparing `poaster-1.3.0/tests/core/test_config.py` & `poaster-1.4.0/tests/core/test_config.py`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/LICENSE` & `poaster-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poaster-1.3.0/README.md` & `poaster-1.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,30 @@
 
 ---
 
 [![builds.sr.ht status](https://builds.sr.ht/~loges/poaster.svg)](https://builds.sr.ht/~loges/poaster?)
 [![PyPI - Version](https://img.shields.io/pypi/v/poaster.svg)](https://pypi.org/project/poaster)
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 
-Minimal, libre bulletin board for posts.
+> Minimal, libre bulletin board for posts.
+
+You can see a simple demo of poaster [here](https://poaster.loganconnolly.com).
+
+## Features
+
+- Display bulletin posts to all users.
+- Create, update, and delete posts as authenticated user.
+- Manage posts through web app and JSON API.
+- Offer CLI for managing users and app state.
+- Expose configuration options through environment variables.
+
+## Roadmap
+
+- Refined access control (admin, members, public).
+- Add markdown support for post content.
 
 ## Quickstart
 
 Install package:
 
 ```console
 pip install poaster
@@ -48,15 +63,14 @@
 # Security
 SECRET_KEY="<generated-when-initializing-app>"
 SECRET_KEY_N_BYTES=32
 ALGORITHM="HS256"
 
 # Theming
 TITLE="poaster"
-POST_SNIPPET_MAX_WORD_COUNT=20
 COLOR_DANGER="#FF595E"
 COLOR_INFO="#1982C4"
 COLOR_PRIMARY="#6A4C93"
 COLOR_SUCCESS="#8AC926"
 COLOR_WARINING="#FFCA3A"
 ```
```

### Comparing `poaster-1.3.0/pyproject.toml` & `poaster-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 ]
 dependencies = [
   "aiosqlite",
   "alembic",
   "click",
   "fastapi",
   "haitch",
+  "mistletoe",
   "passlib[argon2]",
   "pydantic-settings",
   "python-jose",
   "python-multipart",
   "sqlalchemy[asyncio,mypy]",
   "uvicorn[standard]",
 ]
@@ -121,8 +122,9 @@
 select = ["E", "F", "I", "B", "PIE"]
 ignore = []
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 env = [
     "DB_PATH=/:memory:",
+    "SECRET_KEY=super-secure-key",
 ]
```

### Comparing `poaster-1.3.0/PKG-INFO` & `poaster-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: poaster
-Version: 1.3.0
+Version: 1.4.0
 Summary: Minimal, libre bulletin board for posts.
 Project-URL: Homepage, https://sr.ht/~loges/poaster
 Project-URL: Source, https://git.sr.ht/~loges/poaster
 Project-URL: Issues, https://todo.sr.ht/~loges/poaster
 Author-email: Logan Connolly <me@loganconnolly.com>
 License-Expression: AGPL-3.0-or-later
 License-File: LICENSE
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
 Requires-Dist: aiosqlite
 Requires-Dist: alembic
 Requires-Dist: click
 Requires-Dist: fastapi
 Requires-Dist: haitch
+Requires-Dist: mistletoe
 Requires-Dist: passlib[argon2]
 Requires-Dist: pydantic-settings
 Requires-Dist: python-jose
 Requires-Dist: python-multipart
 Requires-Dist: sqlalchemy[asyncio,mypy]
 Requires-Dist: uvicorn[standard]
 Description-Content-Type: text/markdown
@@ -34,15 +35,30 @@
 
 ---
 
 [![builds.sr.ht status](https://builds.sr.ht/~loges/poaster.svg)](https://builds.sr.ht/~loges/poaster?)
 [![PyPI - Version](https://img.shields.io/pypi/v/poaster.svg)](https://pypi.org/project/poaster)
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 
-Minimal, libre bulletin board for posts.
+> Minimal, libre bulletin board for posts.
+
+You can see a simple demo of poaster [here](https://poaster.loganconnolly.com).
+
+## Features
+
+- Display bulletin posts to all users.
+- Create, update, and delete posts as authenticated user.
+- Manage posts through web app and JSON API.
+- Offer CLI for managing users and app state.
+- Expose configuration options through environment variables.
+
+## Roadmap
+
+- Refined access control (admin, members, public).
+- Add markdown support for post content.
 
 ## Quickstart
 
 Install package:
 
 ```console
 pip install poaster
@@ -80,15 +96,14 @@
 # Security
 SECRET_KEY="<generated-when-initializing-app>"
 SECRET_KEY_N_BYTES=32
 ALGORITHM="HS256"
 
 # Theming
 TITLE="poaster"
-POST_SNIPPET_MAX_WORD_COUNT=20
 COLOR_DANGER="#FF595E"
 COLOR_INFO="#1982C4"
 COLOR_PRIMARY="#6A4C93"
 COLOR_SUCCESS="#8AC926"
 COLOR_WARINING="#FFCA3A"
 ```
```

