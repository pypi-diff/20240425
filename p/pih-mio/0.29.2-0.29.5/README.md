# Comparing `tmp/pih-mio-0.29.2.tar.gz` & `tmp/pih-mio-0.29.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mio-0.29.2.tar", last modified: Wed Apr 24 03:32:59 2024, max compression
+gzip compressed data, was "pih-mio-0.29.5.tar", last modified: Thu Apr 25 05:26:58 2024, max compression
```

## Comparing `pih-mio-0.29.2.tar` & `pih-mio-0.29.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 03:32:59.452346 pih-mio-0.29.2/
-drwxrwxrwx   0        0        0        0 2024-04-24 03:32:58.552842 pih-mio-0.29.2/MobileHelperService/
--rw-rw-rw-   0        0        0        0 2024-01-09 05:16:13.000000 pih-mio-0.29.2/MobileHelperService/__init__.py
--rw-rw-rw-   0        0        0      208 2024-02-09 05:31:09.000000 pih-mio-0.29.2/MobileHelperService/__main__.py
--rw-rw-rw-   0        0        0   371457 2024-04-24 03:32:14.000000 pih-mio-0.29.2/MobileHelperService/api.py
--rw-rw-rw-   0        0        0     5945 2024-04-10 05:33:19.000000 pih-mio-0.29.2/MobileHelperService/client.py
--rw-rw-rw-   0        0        0      100 2024-02-20 01:16:51.000000 pih-mio-0.29.2/MobileHelperService/collection.py
--rw-rw-rw-   0        0        0     4465 2024-04-24 03:32:22.000000 pih-mio-0.29.2/MobileHelperService/const.py
--rw-rw-rw-   0        0        0      635 2024-02-14 02:40:54.000000 pih-mio-0.29.2/MobileHelperService/service.py
--rw-rw-rw-   0        0        0    16542 2024-04-23 06:08:38.000000 pih-mio-0.29.2/MobileHelperService/service_api.py
--rw-rw-rw-   0        0        0      331 2024-04-24 03:32:59.421108 pih-mio-0.29.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-24 03:32:59.341974 pih-mio-0.29.2/pih_mio.egg-info/
--rw-rw-rw-   0        0        0      331 2024-04-24 03:32:57.000000 pih-mio-0.29.2/pih_mio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2024-04-24 03:32:57.000000 pih-mio-0.29.2/pih_mio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 03:32:57.000000 pih-mio-0.29.2/pih_mio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-24 03:32:57.000000 pih-mio-0.29.2/pih_mio.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2024-04-24 03:32:57.000000 pih-mio-0.29.2/pih_mio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-24 03:32:57.000000 pih-mio-0.29.2/pih_mio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 03:32:59.500324 pih-mio-0.29.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-25 05:26:58.157224 pih-mio-0.29.5/
+drwxrwxrwx   0        0        0        0 2024-04-25 05:26:57.741736 pih-mio-0.29.5/MobileHelperService/
+-rw-rw-rw-   0        0        0        0 2024-01-09 05:16:13.000000 pih-mio-0.29.5/MobileHelperService/__init__.py
+-rw-rw-rw-   0        0        0      208 2024-02-09 05:31:09.000000 pih-mio-0.29.5/MobileHelperService/__main__.py
+-rw-rw-rw-   0        0        0   371077 2024-04-25 04:56:03.000000 pih-mio-0.29.5/MobileHelperService/api.py
+-rw-rw-rw-   0        0        0     5945 2024-04-10 05:33:19.000000 pih-mio-0.29.5/MobileHelperService/client.py
+-rw-rw-rw-   0        0        0      100 2024-02-20 01:16:51.000000 pih-mio-0.29.5/MobileHelperService/collection.py
+-rw-rw-rw-   0        0        0     4462 2024-04-25 05:26:24.000000 pih-mio-0.29.5/MobileHelperService/const.py
+-rw-rw-rw-   0        0        0      635 2024-02-14 02:40:54.000000 pih-mio-0.29.5/MobileHelperService/service.py
+-rw-rw-rw-   0        0        0    17336 2024-04-25 04:48:36.000000 pih-mio-0.29.5/MobileHelperService/service_api.py
+-rw-rw-rw-   0        0        0      331 2024-04-25 05:26:58.110334 pih-mio-0.29.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 05:26:58.063430 pih-mio-0.29.5/pih_mio.egg-info/
+-rw-rw-rw-   0        0        0      331 2024-04-25 05:26:56.000000 pih-mio-0.29.5/pih_mio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2024-04-25 05:26:57.000000 pih-mio-0.29.5/pih_mio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 05:26:56.000000 pih-mio-0.29.5/pih_mio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-25 05:26:56.000000 pih-mio-0.29.5/pih_mio.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2024-04-25 05:26:56.000000 pih-mio-0.29.5/pih_mio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-25 05:26:56.000000 pih-mio-0.29.5/pih_mio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 05:26:58.157224 pih-mio-0.29.5/setup.cfg
```

### Comparing `pih-mio-0.29.2/MobileHelperService/api.py` & `pih-mio-0.29.5/MobileHelperService/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,15 +367,15 @@
         text: str,
         text_before: str | None = None,
         text_after: str | None = None,
     ) -> str:
         return text
 
     def whatsapp_send(self, text: str) -> bool:
-        A.L.debug_bot(text)
+        #A.L.debug_bot(text)
         return A.ME_WH_W.send(self.get_recipient(), text, self.profile)
 
     @contextmanager
     def make_send_to_group(self, group: A.CT.MESSAGE.WHATSAPP.GROUP):
         try:
             while_not_do(lambda: e(self.message_buffer))
             self.recipient = A.D.get(group)
@@ -5499,23 +5499,14 @@
     def who_lost_the_mark_handler(self) -> None:
         self.console_apps_api.who_lost_the_mark(self.arg())
 
     def marketer_review_statistics_handler(self) -> None:
         self.execute_python_file(
             "marketer_statistics_create",
             redirect_to_mobile_output=True,
-            loading_text="Создание статистики. Ожидайте",
-        )
-        self.output.write_image(
-            "Статистика по отзывам",
-            A.D_CO.file_to_base64(
-                A.PTH_STAT.get_file_path(
-                    A.CT_STAT.Types.POLIBASE_PERSON_REVIEW_NOTIFICATION
-                )
-            ),
         )
         # A.R_F.execute("doctor_list_review_partipant")
 
     def marketer_review_settings_handler(self) -> None:
         def show_settings() -> None:
             self.write_line(
                 js(
@@ -5566,15 +5557,15 @@
             if self.argless and self.yes_no(
                 "Получить отчет в период с начала месяца до сегодняшнего дня"
             ):
                 now: datetime = A.D.now()
                 self.arg_list.append(jp((1, now.month, today.year)))
                 self.arg_list.append(jp((now.day, now.month, today.year)))
 
-        start_date, end_date = self.input.start_and_end_date(self.arg(), self.arg(1))
+        start_date, end_date = self.input.date_period(self.arg(), self.arg(1))
         start_date_string: str = A.D.date_to_string(
             start_date, A.CT.YEARLESS_DATE_FORMAT
         )
         end_date_string: str = A.D.date_to_string(end_date, A.CT.YEARLESS_DATE_FORMAT)
 
         report_file_name: str = A.PTH.add_extension(
             j([self.session.login, start_date_string, end_date_string], "_"),
```

### Comparing `pih-mio-0.29.2/MobileHelperService/client.py` & `pih-mio-0.29.5/MobileHelperService/client.py`

 * *Files identical despite different names*

### Comparing `pih-mio-0.29.2/MobileHelperService/const.py` & `pih-mio-0.29.5/MobileHelperService/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 NAME: str = "MobileHelper"
 
 DEFAULT_COUNT = 100
 ADMIN_ALIAS: str = "admin"
 COUNT_ALIAS: str = "count"
-VERSION: str = "0.29.2"
+VERSION: str = "0.29.5"
 
 HOST = Hosts.WS255
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Mobile helper service",
     host=HOST.NAME,
@@ -147,9 +147,9 @@
 
 ADMIN_GROUPS: list[Groups] = [Groups.Admin]
 
 COMMAND_NAME_VARIANT_SPLITTER: str = "|"
 
 WORKSTATION_CHECK_WORD: str = "Workstation"
 
-VERSION_STRING: str = js((VERSION, "⚙️"))
+VERSION_STRING: str = js((VERSION, "☔"))
 MODULE_NAME: str = j((A.root.NAME, "mio"), "-")
```

### Comparing `pih-mio-0.29.2/MobileHelperService/service.py` & `pih-mio-0.29.5/MobileHelperService/service.py`

 * *Files identical despite different names*

### Comparing `pih-mio-0.29.2/MobileHelperService/service_api.py` & `pih-mio-0.29.5/MobileHelperService/service_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     e,
     nn,
     nl,
     js,
     ne,
     lw,
     one,
+    nnt,
     if_else,
     ParameterList,
     BitMask as BM,
 )
 from pih.collections import WhatsAppMessage, User, Message
 from pih.collections.service import ServiceDescription, SubscribtionResult
 
@@ -37,32 +38,34 @@
 from collections import defaultdict
 from typing import Callable, Any
 
 SC = A.CT_SC
 
 ISOLATED: bool = False
 
+ADMIN_LOGIN: str = "nak"
+
 
 def sender_is_cli(value: str) -> bool:
     return value in A.D.map(
         lambda item: item[1],
         A.D.filter(
             lambda item: item[0].lower().endswith("cli"),
-            A.D.to_list(A.CT_ME_WH.GROUP, None), # type: ignore
+            A.D.to_list(A.CT_ME_WH.GROUP, None),  # type: ignore
         ),
     )
 
 
 class MobileHelperService:
 
     is_admin: bool = False
 
     @staticmethod
     def as_admin() -> bool:
-        return MobileHelperService.is_admin or not A.D.contains(A.SYS.host(), SD.host) # type: ignore
+        return MobileHelperService.is_admin or not A.D.contains(A.SYS.host(), SD.host)  # type: ignore
 
     @staticmethod
     def count() -> int:
         return A.SE.named_arg(COUNT_ALIAS)  # type: ignore
 
     mobile_helper_client_map: dict[str, Api] = {}
 
@@ -90,19 +93,29 @@
             MobileHelperService.is_admin = lw(A.SE.named_arg(ADMIN_ALIAS)) in [
                 "1",
                 "true",
                 "yes",
             ]
         else:
             MobileHelperService.is_admin = False
+
+        def service_starts_handler() -> None:
+            if MobileHelperService.as_admin():
+                self.create_mobile_helper(
+                    A.D.get(A.CT_ME_WH_G.PIH_CLI),
+                    None,
+                    A.D_U.by_login(ADMIN_LOGIN).telephoneNumber,
+                )
+            MobileHelperService.service_starts_handler()
+
         if ne(service_desctiption):
             A.SRV_A.serve(
                 service_desctiption,
-                self.service_call_handler,
-                MobileHelperService.service_starts_handler,
+                self.service_call_handler,  # type: ignore
+                service_starts_handler,
                 as_standalone=as_standalone,
                 isolate=ISOLATED,
             )
             return True
         return False
 
     def create_mobile_helper(
@@ -115,67 +128,69 @@
         if is_cli:
             external_flags = BM.add(external_flags, Flags.CLI)
         stdin: Stdin = Stdin()
         session: MobileSession = MobileSession(sender, external_flags)
         output: MobileOutput = MobileOutput(session)
         try:
             session.say_hello(recipient)
-            output.write_line(
-                j(
-                    (
+            if not is_cli:
+                output.write_line(
+                    j(
                         (
-                            j(
-                                (
-                                    "Добро пожаловать, ",
-                                    nl(
-                                        j(
-                                            (
-                                                output.user.get_formatted_given_name(
-                                                    session.user_given_name
-                                                ),
-                                                "!",
+                            (
+                                j(
+                                    (
+                                        "Добро пожаловать, ",
+                                        nl(
+                                            j(
+                                                (
+                                                    output.user.get_formatted_given_name(
+                                                        session.user_given_name
+                                                    ),
+                                                    "!",
+                                                )
                                             )
-                                        )
-                                    ),
+                                        ),
+                                    )
                                 )
-                            )
-                            if not BM.has(session.flags, Flags.ONLY_RESULT)
-                            else None
-                        ),
-                        " ",
-                        A.CT_V.WAIT,
-                        " ",
-                        i("Ожидайте..."),
+                                if not BM.has(session.flags, Flags.ONLY_RESULT)
+                                else None
+                            ),
+                            " ",
+                            A.CT_V.WAIT,
+                            " ",
+                            i("Ожидайте..."),
+                        )
                     )
                 )
-            )
         except NotFound as error:
             output.error(
                 "К сожалению, не могу идентифицировать Вас. ИТ отдел добавит Вас после окончания процедуры идентификации."
             )
             raise error
         as_admin: bool = is_cli
         if not as_admin:
             try:
                 as_admin = A.C_U.by_group(
-                    A.R_U.by_telephone_number(sender).data, A.CT_AD.Groups.Admin # type: ignore
+                    nnt(A.R_U.by_telephone_number(sender).data), A.CT_AD.Groups.Admin
                 )
             except NotFound as _:
                 pass
         input: MobileInput = MobileInput(
             stdin,
             MobileUserInput(),
             MobileMarkInput(),
             output,
             session,
             [None, -1][as_admin],
         )
         api: Api = Api(PIH(input, output, session), stdin)
         if is_cli:
             api.external_flags = external_flags
+        MobileHelperService.mobile_helper_client_map[sender] = api
         return api
 
     @staticmethod
     def say_good_bye(mobile_helper: Api, with_error: bool = False) -> None:
         mobile_helper.say_good_bye(with_error=with_error)
         mobile_helper.show_good_bye = False
 
@@ -196,54 +211,52 @@
                 if MobileHelperService.is_client_new(sender):
                     A.IW.remove(A.CT_P.NAMES.PERSON_PIN, sender)
                     if is_cli or Api.check_for_starts_with_pih_keyword(line):
                         self.allow_send_to_next_service_in_chain[sender] = (
                             self.is_client_stack_full()
                         )
                         if not self.allow_send_to_next_service_in_chain[sender]:
-                            MobileHelperService.mobile_helper_client_map[sender] = (
-                                self.create_mobile_helper(
-                                    sender, external_flags, chat_id
-                                )
-                            )
+                            self.create_mobile_helper(sender, external_flags, chat_id)
                     else:
                         self.allow_send_to_next_service_in_chain[sender] = False
                 else:
                     self.allow_send_to_next_service_in_chain[sender] = False
                 if sender in MobileHelperService.mobile_helper_client_map:
                     mobile_helper = MobileHelperService.mobile_helper_client_map[sender]
                     if is_cli and not mobile_helper.wait_for_input():
                         if not Api.check_for_starts_with_pih_keyword(line):
                             line = js((self.root, line))
                     try:
                         if mobile_helper.do_pih(
-                            line, sender_user, external_flags, return_result_key, args # type: ignore
+                            line, sender_user, external_flags, return_result_key, args  # type: ignore
                         ):
                             if mobile_helper.show_good_bye:
                                 if not mobile_helper.is_only_result:
                                     MobileHelperService.say_good_bye(mobile_helper)
                     except BaseException as error:
                         is_error: bool = not isinstance(error, InternalInterrupt)
                         if not mobile_helper.is_only_result and is_error:
-                            MobileHelperService.say_good_bye(mobile_helper, with_error = is_error)
+                            MobileHelperService.say_good_bye(
+                                mobile_helper, with_error=is_error
+                            )
                         raise error
                 break
             except NotFound:
                 break
             except InternalInterrupt as interruption:
                 if interruption.type == InterruptionTypes.NEW_COMMAND:
-                    line = mobile_helper.line
+                    line = nnt(mobile_helper).line
                     if not Api.check_for_starts_with_pih_keyword(line):
-                        MobileHelperService.say_good_bye(mobile_helper)
+                        MobileHelperService.say_good_bye(nnt(mobile_helper))
                         break
                 elif interruption.type in (
                     InterruptionTypes.TIMEOUT,
                     InterruptionTypes.EXIT,
                 ):
-                    MobileHelperService.say_good_bye(mobile_helper)
+                    MobileHelperService.say_good_bye(nnt(mobile_helper))
                     break
 
     def is_client_stack_full(self) -> bool:
         max_client_count: int | None = self.max_client_count
         if n(max_client_count):
             max_client_count = MobileHelperService.count()
         return len(MobileHelperService.mobile_helper_client_map) == max_client_count
@@ -274,76 +287,81 @@
                         return_result_key,
                         args,
                     )
                 else:
                     for recipient_user in interruption.recipient_user_list():
                         recipient_user: User = recipient_user
                         self.pih_handler(
-                            recipient_user.telephoneNumber,
-                            js((self.root, interruption.command_name)),
-                            interruption.sender_user,
-                            interruption.flags,
+                            nnt(recipient_user.telephoneNumber),
+                            js((self.root, nnt(interruption).command_name)),
+                            nnt(interruption).sender_user,
+                            nnt(interruption).flags,
                         )
                     interruption = None
                 break
             except AddressedInterruption as local_interruption:
                 interruption = local_interruption
 
     def receive_message_handler_thread_handler(self, message: WhatsAppMessage) -> None:
         self.receive_message_handler(
-            message.message,
-            message.sender,
-            message.flags,
-            message.chatId,
-            message.return_result_key,
-            message.args,
+            nnt(nnt(message).message),
+            nnt(nnt(message).sender),
+            nnt(message).flags,
+            nnt(message).chatId,
+            nnt(message).return_result_key,
+            nnt(message).args,
         )
 
     def service_call_handler(
         self,
         sc: SC,
         parameter_list: ParameterList,
         subscribtion_result: SubscribtionResult | None,
     ) -> Any:
         if sc == A.CT_SC.send_event:
-            if nn(subscribtion_result) and subscribtion_result.result:
-                if subscribtion_result.type == A.CT_SubT.ON_RESULT_SEQUENTIALLY:
+            if nn(subscribtion_result) and nnt(subscribtion_result).result:
+                if nnt(subscribtion_result).type == A.CT_SubT.ON_RESULT_SEQUENTIALLY:
                     message: WhatsAppMessage | None = A.D_Ex_E.whatsapp_message(
                         parameter_list
                     )
 
                     if nn(message):
                         if (
-                            A.D.get_by_value(A.CT_ME_WH_W.Profiles, message.profile_id)
+                            A.D.get_by_value(
+                                A.CT_ME_WH_W.Profiles, nnt(message).profile_id
+                            )
                             == A.CT_ME_WH_W.Profiles.IT
                         ):
                             allow_for_group: bool = ne(
-                                message.chatId
-                            ) and sender_is_cli(message.chatId)
-                            if n(message.chatId) or allow_for_group:
+                                nnt(message).chatId
+                            ) and sender_is_cli(nnt(nnt(message).chatId))
+                            if n(nnt(message).chatId) or allow_for_group:
                                 telephone_number: str = if_else(
-                                    allow_for_group, message.chatId, message.sender
+                                    allow_for_group,
+                                    nnt(message).chatId,
+                                    nnt(message).sender,
                                 )
                                 if allow_for_group:
-                                    message.chatId = message.sender
-                                    message.sender = telephone_number
+                                    nnt(message).chatId = nnt(message).sender
+                                    nnt(message).sender = telephone_number
                                 if n(self.checker) or self.checker(telephone_number):
                                     if self.is_client_stack_full():
                                         return True
                                     else:
                                         if (
                                             telephone_number
                                             in self.allow_send_to_next_service_in_chain
                                         ):
                                             del self.allow_send_to_next_service_in_chain[
                                                 telephone_number
                                             ]
                                         PIHThread(
                                             self.receive_message_handler_thread_handler,
-                                            args=[message], name="receive_message_handler_thread_handler"
+                                            args=[message],
+                                            name="receive_message_handler_thread_handler",
                                         )
                                         while (
                                             telephone_number
                                             not in self.allow_send_to_next_service_in_chain
                                         ):
                                             pass
                                         return self.allow_send_to_next_service_in_chain[
@@ -397,13 +415,13 @@
                             nl() * 2,
                             get_wappi_status(space, profile.CALL_CENTRE),
                             nl() * 2,
                             get_wappi_status(space, profile.MARKETER),
                         )
                     ),
                     A.D.get(A.CT_ME_WH.GROUP.PIH_CLI),
-                    A.D.get(profile.IT)
+                    A.D.get(profile.IT),
                 )
             )
 
         for item in one(A.R_F.find("@mobile_helper_import_module_list")).text.splitlines():  # type: ignore
             A.R_F.execute(item)
```

