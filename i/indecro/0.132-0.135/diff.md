# Comparing `tmp/indecro-0.132.tar.gz` & `tmp/indecro-0.135.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indecro-0.132.tar", last modified: Fri May 26 08:59:40 2023, max compression
+gzip compressed data, was "indecro-0.135.tar", last modified: Sat Jun 10 07:16:21 2023, max compression
```

## Comparing `indecro-0.132.tar` & `indecro-0.135.tar`

### file list

```diff
@@ -1,22 +1,36 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-26 08:59:40.899741 indecro-0.132/
--rw-r--r--   0 user      (1000) user      (1000)     1069 2023-05-25 02:33:35.000000 indecro-0.132/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     2070 2023-05-26 08:59:40.899741 indecro-0.132/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1536 2023-05-26 08:51:44.000000 indecro-0.132/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-26 08:59:40.898741 indecro-0.132/indecro/
--rw-r--r--   0 user      (1000) user      (1000)       33 2023-05-25 03:11:46.000000 indecro-0.132/indecro/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      898 2023-05-26 03:50:28.000000 indecro-0.132/indecro/exceptions.py
--rw-r--r--   0 user      (1000) user      (1000)     1701 2023-05-25 09:16:34.000000 indecro-0.132/indecro/executor.py
--rw-r--r--   0 user      (1000) user      (1000)     1531 2023-05-26 03:53:49.000000 indecro-0.132/indecro/job.py
--rw-r--r--   0 user      (1000) user      (1000)     3352 2023-05-26 06:06:40.000000 indecro-0.132/indecro/rules.py
--rw-r--r--   0 user      (1000) user      (1000)     3703 2023-05-26 08:58:07.000000 indecro-0.132/indecro/scheduler.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-26 08:59:40.899741 indecro-0.132/indecro/storage/
--rw-r--r--   0 user      (1000) user      (1000)       41 2023-05-25 03:46:12.000000 indecro-0.132/indecro/storage/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     2126 2023-05-23 18:24:15.000000 indecro-0.132/indecro/storage/base.py
--rw-r--r--   0 user      (1000) user      (1000)     1113 2023-05-26 04:29:00.000000 indecro-0.132/indecro/storage/memory_storage.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-26 08:59:40.899741 indecro-0.132/indecro.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     2070 2023-05-26 08:59:40.000000 indecro-0.132/indecro.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      361 2023-05-26 08:59:40.000000 indecro-0.132/indecro.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-26 08:59:40.000000 indecro-0.132/indecro.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)        8 2023-05-26 08:59:40.000000 indecro-0.132/indecro.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       79 2023-05-26 08:59:40.899741 indecro-0.132/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      936 2023-05-26 08:59:40.000000 indecro-0.132/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-10 07:16:21.053787 indecro-0.135/
+-rw-r--r--   0 user      (1000) user      (1000)     1069 2023-05-25 02:33:35.000000 indecro-0.135/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     2070 2023-06-10 07:16:21.053787 indecro-0.135/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1536 2023-05-26 08:51:44.000000 indecro-0.135/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-10 07:16:21.052787 indecro-0.135/indecro/
+-rw-r--r--   0 user      (1000) user      (1000)       33 2023-05-25 03:11:46.000000 indecro-0.135/indecro/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-10 07:16:21.052787 indecro-0.135/indecro/api/
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-06-10 06:27:47.000000 indecro-0.135/indecro/api/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      312 2023-06-10 06:57:00.000000 indecro-0.135/indecro/api/executor.py
+-rw-r--r--   0 user      (1000) user      (1000)     1072 2023-06-10 06:44:48.000000 indecro-0.135/indecro/api/job.py
+-rw-r--r--   0 user      (1000) user      (1000)     2715 2023-06-10 07:12:13.000000 indecro-0.135/indecro/api/rules.py
+-rw-r--r--   0 user      (1000) user      (1000)     1485 2023-06-10 06:57:25.000000 indecro-0.135/indecro/api/scheduler.py
+-rw-r--r--   0 user      (1000) user      (1000)     2584 2023-06-10 07:14:23.000000 indecro-0.135/indecro/api/storage.py
+-rw-r--r--   0 user      (1000) user      (1000)      101 2023-05-23 19:03:46.000000 indecro-0.135/indecro/api/task.py
+-rw-r--r--   0 user      (1000) user      (1000)       21 2023-05-29 13:48:25.000000 indecro-0.135/indecro/defaults.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-10 07:16:21.053787 indecro-0.135/indecro/exceptions/
+-rw-r--r--   0 user      (1000) user      (1000)       39 2023-06-10 07:07:04.000000 indecro-0.135/indecro/exceptions/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)       44 2023-06-10 07:05:50.000000 indecro-0.135/indecro/exceptions/base.py
+-rw-r--r--   0 user      (1000) user      (1000)      198 2023-06-10 07:07:04.000000 indecro-0.135/indecro/exceptions/job.py
+-rw-r--r--   0 user      (1000) user      (1000)      837 2023-06-10 07:07:04.000000 indecro-0.135/indecro/exceptions/rule.py
+-rw-r--r--   0 user      (1000) user      (1000)      296 2023-06-10 07:07:04.000000 indecro-0.135/indecro/exceptions/scheduler.py
+-rw-r--r--   0 user      (1000) user      (1000)     1709 2023-06-10 06:32:26.000000 indecro-0.135/indecro/executor.py
+-rw-r--r--   0 user      (1000) user      (1000)     1509 2023-06-10 07:14:31.000000 indecro-0.135/indecro/job.py
+-rw-r--r--   0 user      (1000) user      (1000)     3969 2023-06-10 07:07:53.000000 indecro-0.135/indecro/rules.py
+-rw-r--r--   0 user      (1000) user      (1000)     4081 2023-06-10 07:08:30.000000 indecro-0.135/indecro/scheduler.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-10 07:16:21.053787 indecro-0.135/indecro/storage/
+-rw-r--r--   0 user      (1000) user      (1000)       41 2023-05-25 03:46:12.000000 indecro-0.135/indecro/storage/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2714 2023-06-10 07:09:27.000000 indecro-0.135/indecro/storage/base.py
+-rw-r--r--   0 user      (1000) user      (1000)     1199 2023-06-10 06:44:48.000000 indecro-0.135/indecro/storage/memory_storage.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-10 07:16:21.052787 indecro-0.135/indecro.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     2070 2023-06-10 07:16:21.000000 indecro-0.135/indecro.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      658 2023-06-10 07:16:21.000000 indecro-0.135/indecro.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-06-10 07:16:21.000000 indecro-0.135/indecro.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)        8 2023-06-10 07:16:21.000000 indecro-0.135/indecro.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       79 2023-06-10 07:16:21.053787 indecro-0.135/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      861 2023-06-10 07:15:36.000000 indecro-0.135/setup.py
```

### Comparing `indecro-0.132/LICENSE` & `indecro-0.135/LICENSE`

 * *Files identical despite different names*

### Comparing `indecro-0.132/PKG-INFO` & `indecro-0.135/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indecro
-Version: 0.132
+Version: 0.135
 Summary: Python scheduler with task independency from scheduler, executor and others
 Home-page: https://github.com/TypeHintsFun/indecro
 Author: TypeHintsFun
 Author-email: typehintsfun@gmail.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `indecro-0.132/README.md` & `indecro-0.135/README.md`

 * *Files identical despite different names*

### Comparing `indecro-0.132/indecro/executor.py` & `indecro-0.135/indecro/executor.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from indecro.api.job import Job, RunAs
 
 
 class Executor(ExecutorProtocol):
     def __init__(self):
         self.daemonized_tasks: set[asyncio.Task] = set()
 
-    async def execute(self, job: Job):
+    async def execute(self, job: Job) -> bool:
         if job.is_running:
             return False
 
         if job.daemonize is RunAs.FUNCTION:
             res = self.sync_worker(job.task, job)
 
             if isinstance(res, Awaitable):
```

### Comparing `indecro-0.132/indecro/job.py` & `indecro-0.135/indecro/job.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,41 +8,44 @@
 from indecro.api.task import Task
 from indecro.api.rules import Rule, BoolRule
 from indecro.api.scheduler import Scheduler
 from indecro.api.job import Job as JobProtocol, RunAs
 
 
 @dataclass
-class Job(JobProtocol):  # If the Job is highlighted in red, the bad work of the paycharm with dataclasses and typehints for them is to blame
+class Job(JobProtocol):  # If the Job is highlighted in red, the bad work of the paycharm with dataclasses and
+    # typehints for them is to blame
     task: Task
     rule: Union[Rule, BoolRule]
 
     next_run_time: datetime
 
     daemonize: RunAs = RunAs.FUNCTION
 
-    name: Optional[str] = None
+    id: Optional[str] = None
 
     is_running: bool = False
 
     scheduler: Optional[Scheduler] = None
     executor: Optional[Executor] = None
 
     running_task: Optional[asyncio.Task] = None
 
-    async def schedule(self, reschedule: bool = True) -> None:
+    def schedule(self) -> None:
         if self.scheduler is None:
             raise ValueError('To use schedule shortcut you must provide an scheduler attribute for job object')
 
-        await self.scheduler.schedule_job(self)
+        self.scheduler.schedule_job(self)
 
-    async def execute(self, reschedule: bool = True) -> Any:
+    async def execute(self, reschedule: bool = True) -> bool:
         if self.executor is None:
             raise ValueError('To use execute shortcut you must provide an executor attribute for job object')
 
-        await self.executor.execute(self)
+        executed = await self.executor.execute(self)
 
         if reschedule:
-            await self.scheduler.schedule_job(self)
+            self.schedule()
+
+        return executed
 
     def __hash__(self):
-        return hash(hash(self.rule) + hash(self.name) + hash(self.task))
+        return hash(hash(self.rule) + hash(self.id) + hash(self.task))
```

### Comparing `indecro-0.132/indecro/rules.py` & `indecro-0.135/indecro/rules.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from dataclasses import dataclass, field
 from datetime import datetime, timedelta
 from typing import Optional, Callable, Any, Union
 
 from magic_filter import MagicFilter
 
-from indecro.api.rules import Rule, BoolRule
-from indecro.exceptions import JobNeverBeScheduled
+from indecro.api.rules import Rule, BoolRule, CheckEvery
+
+from indecro.defaults import SECONDS_PER_LOOP
+from indecro.exceptions.rule import JobNeverBeScheduled
 
 
 @dataclass
 class RunEvery(Rule):
     period: timedelta
     after: Optional[Union[datetime, timedelta]] = None
     before: Optional[Union[datetime, timedelta]] = None
@@ -20,15 +22,15 @@
     repeats: int = 0
 
     def get_next_schedule_time(self, *, after: datetime) -> datetime:
         # Lazy after timedelta to datetime transformation instead of __init__ redefinition
         if isinstance(self.after, timedelta):
             self.after = self.init_time + self.after
 
-        #similar actions for before
+        # similar actions for before
         if isinstance(self.before, timedelta):
             self.before = self.init_time + self.before
 
         delta = after - self.init_time
         intervals = delta.total_seconds() // self.period.total_seconds() + 1
 
         next_schedule_time = self.init_time + intervals * self.period
@@ -51,19 +53,23 @@
         # TODO: Remove hardcode from arguments displaying in repr
         return f'{self.__class__.__name__}(start={repr(self.after)}, period={repr(self.period)})'
 
     def __hash__(self):
         return hash(repr(self))
 
 
+# Execute job just one time
 @dataclass(init=False)
 class RunOnce(Rule):
     at: Optional[datetime] = None
+    # time_to_execute = at
     after: Optional[timedelta] = None
 
+    # time_to_execute = now + after
+
     def __init__(
             self,
             at: Optional[datetime] = None,
             after: Optional[timedelta] = None
     ):
         if (not at) and (not after):
             raise ValueError('You must provide at parameter or after parameter')
@@ -83,24 +89,40 @@
         # TODO: Remove hardcode from arguments displaying in repr
         return f'{self.__class__.__name__}(at={repr(self.at)}, after={self.after})'
 
     def __hash__(self):
         return hash(repr(self))
 
 
+# The most useful BoolRule realisation example
 @dataclass
 class RunWhen(BoolRule):
     will: Union[MagicFilter, Callable[[], bool]]
     subject: Union[None, Any] = None
 
+    repeats: int = -1
+
+    check_every: CheckEvery = CheckEvery(timedelta(seconds=SECONDS_PER_LOOP))
+
+    repeats_passed: int = 0
+
     def get_must_be_scheduled_now_flag(self):
         if isinstance(self.will, MagicFilter):
-            return self.will.resolve(self.subject)
+            res = self.will.resolve(self.subject)
         elif isinstance(self.will, Callable):
-            return self.will()
+            res = self.will()
+        else:
+            res = False
+
+        if res is True:
+            self.repeats_passed += 1
+
+        if self.repeats >= 0 and self.repeats_passed > self.repeats:  # PyCharm, fuck you
+            raise JobNeverBeScheduled(after=datetime.now(), by_rule=self)
+        return res
 
     def __repr__(self):
         # TODO: Remove hardcode from arguments displaying in repr
         return f'{self.__class__.__name__}(at={repr(self.will)}, after={self.subject})'
 
     def __hash__(self):
         return hash(repr(self))
```

### Comparing `indecro-0.132/indecro/scheduler.py` & `indecro-0.135/indecro/scheduler.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,128 +2,139 @@
 import functools
 from datetime import datetime
 from typing import Optional, Union, Awaitable
 
 from indecro.api.executor import Executor
 from indecro.api.job import RunAs
 from indecro.api.task import Task
-from indecro.exceptions import JobNeverBeScheduled, CannotPredictJobSchedulingTime
 from indecro.api.job import Job as JobProtocol
-from indecro.job import Job
 from indecro.api.rules import Rule
 from indecro.api.scheduler import Scheduler as SchedulerProtocol
 from indecro.api.storage import Storage, AsyncStorage
 
+from indecro.defaults import SECONDS_PER_LOOP
+from indecro.exceptions.rule import JobNeverBeScheduled, CannotPredictJobSchedulingTime
+
+from indecro.job import Job
+
 
 class Scheduler(SchedulerProtocol):
     def __init__(
             self,
             storage: Union[Storage, AsyncStorage],
             executor: Executor,
-            loop_delay: Union[int, float] = 1
+            loop_delay: Union[int, float] = SECONDS_PER_LOOP
     ):
         self.storage = storage
         self.executor = executor
 
         self.loop_delay = loop_delay
 
         self.running = False
 
     def job(
             self,
             rule: Rule,
 
             daemonize: RunAs = RunAs.FUNCTION,
 
-            name: Optional[str] = None,
+            id: Optional[str] = None,
 
             *args,
             **kwargs
     ):
         def decorator(task: Task):
             self.add_job(
                 task=task,
                 rule=rule,
                 daemonize=daemonize,
-                name=name,
+                id=id,
                 *args,
                 **kwargs
             )
             return task
 
         return decorator
 
     def add_job(
             self,
             task: Task,
             rule: Rule,
 
             daemonize: RunAs = RunAs.FUNCTION,
 
-            name: Optional[str] = None,
+            id: Optional[str] = None,
             *args,
             **kwargs
     ) -> JobProtocol:
         if isinstance(task, Job):
             job = task
         else:
             try:
                 next_run_time = rule.get_next_schedule_time(after=datetime.now())
             except CannotPredictJobSchedulingTime:
                 next_run_time = None
             job = Job(
                 task=functools.partial(task, *args, **kwargs),
                 rule=rule,
                 next_run_time=next_run_time,
-                name=name,
+                id=id,
                 scheduler=self,
                 executor=self.executor,
                 daemonize=daemonize
             )
 
         return self.storage.add_job(job)
 
     def stop(self):
         self.running = False
 
-    async def execute_job(self, job: JobProtocol, reschedule: bool = True):
-        job_executed = await self.executor.execute(job)
-
-        if reschedule:
-            self.schedule_job(job)
+    async def execute_job(self, job: Union[JobProtocol, str], reschedule: bool = True) -> bool:
+        if isinstance(job, str):
+            job = self.storage.get_job(job)
+            if job is None:
+                raise
+
+        return await job.execute(reschedule=reschedule)
+
+    def schedule_job(self, job: Union[JobProtocol, str]):
+        if isinstance(job, str):
+            job = self.storage.get_job(job)
+            if job is None:
+                raise
 
-        return job_executed
-
-    @staticmethod
-    def schedule_job(job: JobProtocol):
         try:
             job.next_run_time = job.rule.get_next_schedule_time(after=datetime.now())
         except CannotPredictJobSchedulingTime:
             pass
-        return None
 
-    def remove_job(self, job: JobProtocol):
+    def remove_job(self, job: Union[JobProtocol, str]):
+        if isinstance(job, str):
+            job = self.storage.get_job(job)
+            if job is None:
+                raise
+
         return self.storage.remove_job(job)
 
     async def run(self):
         self.running = True
         while self.running:
             now = datetime.now()
 
             any_job_started = False
-            for job in self.storage.iter_jobs(before=now):
+            for job in self.storage.iter_actual_jobs(before=now):
+                job_executed = False  # Setting a default value
+
                 try:
                     job_executed = await self.execute_job(job)
                 except JobNeverBeScheduled:
                     res = self.storage.remove_job(job)
 
                     if isinstance(res, Awaitable):
                         await res
-
-                    job_executed = False
                 except CannotPredictJobSchedulingTime:  # Looks like BoolRule, we just wait
-                    job_executed = False
+                    pass
 
                 any_job_started = job_executed or any_job_started
 
             # Sleeping loop_delay seconds if not any job started, else sleeping 0 seconds (asyncio magic)
             await asyncio.sleep(self.loop_delay * (not any_job_started))
```

### Comparing `indecro-0.132/indecro/storage/base.py` & `indecro-0.135/indecro/storage/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,71 +1,92 @@
 from abc import ABC, abstractmethod
 from datetime import datetime
 
 from typing import Generator, AsyncGenerator, Optional, Union
 
 from indecro.api.job import Job
 from indecro.api.storage import Storage, AsyncStorage
+from indecro.exceptions.job import JobNotFound
 
 
 class BaseStorage(Storage, ABC):
     def get_closest_job(self, *, after: datetime) -> Union[Job, None]:
-        for job in self.iter_jobs(after=after):
+        for job in self.iter_actual_jobs(after=after):
             return job
         return None
 
     def get_duty_job(self, *, before: datetime) -> Union[Job, None]:
-        for job in self.iter_jobs(before=before):
+        for job in self.iter_actual_jobs(before=before):
             return job
         return None
 
+    def get_job(self, job_id: str) -> Job:
+        for job in self:
+            if job.id == job_id:
+                return job
+        raise JobNotFound(by_id=job_id)
+
     @property
     def duty_job(self) -> Union[Job, None]:
         return self.get_duty_job(before=datetime.now())
 
     @property
     def next_job(self) -> Union[Job, None]:
         return self.get_closest_job(after=datetime.now())
 
     @abstractmethod
-    def iter_jobs(
+    def iter_actual_jobs(
             self,
             *,
             after: Optional[datetime] = None,
             before: Optional[datetime] = None,
             limit: Optional[int] = None
     ) -> Generator[Job, None, None]:
         raise NotImplementedError()
 
+    @abstractmethod
+    def __iter__(self):
+        raise NotImplementedError()
+
 
 class BaseAsyncStorage(AsyncStorage, ABC):
     async def get_closest_job(self, *, after: datetime) -> Union[Job, None]:
-        async for job in self.iter_jobs(after=after):
+        async for job in self.iter_actual_jobs(after=after):
             return job
         return None
 
     async def get_duty_job(self, *, before: datetime) -> Union[Job, None]:
-        async for job in self.iter_jobs(before=before):
+        async for job in self.iter_actual_jobs(before=before):
             return job
         return None
 
     @property
     async def duty_job(self) -> Union[Job, None]:
         return await self.get_duty_job(before=datetime.now())
 
     @property
     async def next_job(self) -> Union[Job, None]:
         return await self.get_closest_job(after=datetime.now())
 
     @abstractmethod
-    async def iter_jobs(
+    async def iter_actual_jobs(
             self,
             *,
             after: Optional[datetime] = None,
             before: Optional[datetime] = None,
             limit: Optional[int] = None
     ) -> AsyncGenerator[Job, None]:
         raise NotImplementedError()
         yield  # For generator-like typehints in PyCharm
 
+    async def get_job(self, job_id: str) -> Job:
+        async for job in self:
+            if job.id == job_id:
+                return job
+        return None
+
+    @abstractmethod
+    async def __aiter__(self):
+        raise NotImplementedError()
+
 
 __all__ = ('BaseStorage', 'BaseAsyncStorage')
```

### Comparing `indecro-0.132/indecro/storage/memory_storage.py` & `indecro-0.135/indecro/storage/memory_storage.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 from datetime import datetime
-from typing import Optional, Generator
+from typing import Optional, Generator, Union
 
 from .base import BaseStorage
 from indecro.api.job import Job
 
 
 class MemoryStorage(BaseStorage):
     def __init__(self):
         self.jobs: set[Job] = set()
 
-    def add_job(self, job: Job):
+    def add_job(self, job: Union[Job, str]):
         self.jobs.add(job)
 
-    def remove_job(self, job: Job):
+    def remove_job(self, job: Union[Job, str]):
         self.jobs.remove(job)
 
-    def iter_jobs(
+    def __iter__(self):
+        yield from sorted(self.jobs, key=lambda job: job.next_run_time)
+
+    def iter_actual_jobs(
             self,
             *,
             after: Optional[datetime] = None,
             before: Optional[datetime] = None,
             limit: Optional[int] = None
     ) -> Generator[Job, None, None]:
 
         a = 0
-        for job in sorted(self.jobs, key=lambda job: job.next_run_time):
-
+        for job in self:
             if job.next_run_time is None:
                 if job.rule.get_must_be_scheduled_now_flag():
                     yield job
                     a += 1
             elif (
                     (after is not None and job.next_run_time > after) or
                     (before is not None and job.next_run_time < before)
```

### Comparing `indecro-0.132/indecro.egg-info/PKG-INFO` & `indecro-0.135/indecro.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indecro
-Version: 0.132
+Version: 0.135
 Summary: Python scheduler with task independency from scheduler, executor and others
 Home-page: https://github.com/TypeHintsFun/indecro
 Author: TypeHintsFun
 Author-email: typehintsfun@gmail.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

