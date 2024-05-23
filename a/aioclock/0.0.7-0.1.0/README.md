# Comparing `tmp/aioclock-0.0.7.tar.gz` & `tmp/aioclock-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioclock-0.0.7.tar", max compression
+gzip compressed data, was "aioclock-0.1.0.tar", max compression
```

## Comparing `aioclock-0.0.7.tar` & `aioclock-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,17 @@
--rw-r--r--   0        0        0     1072 2024-05-12 22:38:17.081409 aioclock-0.0.7/LICENSE
--rw-r--r--   0        0        0     3311 2024-05-12 22:38:17.081409 aioclock-0.0.7/README.md
--rw-r--r--   0        0        0      299 2024-05-12 22:38:17.081409 aioclock-0.0.7/aioclock/__init__.py
--rw-r--r--   0        0        0     4561 2024-05-12 22:38:17.085409 aioclock-0.0.7/aioclock/app.py
--rw-r--r--   0        0        0     2146 2024-05-12 22:38:17.085409 aioclock-0.0.7/aioclock/group.py
--rw-r--r--   0        0        0       55 2024-05-12 22:38:17.085409 aioclock-0.0.7/aioclock/logger.py
--rw-r--r--   0        0        0      245 2024-05-12 22:38:17.085409 aioclock-0.0.7/aioclock/provider.py
--rw-r--r--   0        0        0     1374 2024-05-12 22:38:17.085409 aioclock-0.0.7/aioclock/task.py
--rw-r--r--   0        0        0    12544 2024-05-12 22:38:17.085409 aioclock-0.0.7/aioclock/triggers.py
--rw-r--r--   0        0        0     1042 2024-05-12 22:38:17.085409 aioclock-0.0.7/aioclock/types.py
--rw-r--r--   0        0        0      862 2024-05-12 22:38:17.085409 aioclock-0.0.7/aioclock/utils.py
--rw-r--r--   0        0        0     2014 2024-05-12 22:38:39.689321 aioclock-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     4254 1970-01-01 00:00:00.000000 aioclock-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-23 20:18:50.277093 aioclock-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3311 2024-05-23 20:18:50.277093 aioclock-0.1.0/README.md
+-rw-r--r--   0        0        0      322 2024-05-23 20:18:50.277093 aioclock-0.1.0/aioclock/__init__.py
+-rw-r--r--   0        0        0     4430 2024-05-23 20:18:50.277093 aioclock-0.1.0/aioclock/api.py
+-rw-r--r--   0        0        0     5392 2024-05-23 20:18:50.277093 aioclock-0.1.0/aioclock/app.py
+-rw-r--r--   0        0        0      172 2024-05-23 20:18:50.277093 aioclock-0.1.0/aioclock/exceptions.py
+-rw-r--r--   0        0        0      388 2024-05-23 20:18:50.277093 aioclock-0.1.0/aioclock/ext/__init__.py
+-rw-r--r--   0        0        0     2667 2024-05-23 20:18:50.277093 aioclock-0.1.0/aioclock/ext/fastapi.py
+-rw-r--r--   0        0        0     2422 2024-05-23 20:18:50.277093 aioclock-0.1.0/aioclock/group.py
+-rw-r--r--   0        0        0       55 2024-05-23 20:18:50.277093 aioclock-0.1.0/aioclock/logger.py
+-rw-r--r--   0        0        0      245 2024-05-23 20:18:50.277093 aioclock-0.1.0/aioclock/provider.py
+-rw-r--r--   0        0        0     2303 2024-05-23 20:18:50.277093 aioclock-0.1.0/aioclock/task.py
+-rw-r--r--   0        0        0    15310 2024-05-23 20:18:50.277093 aioclock-0.1.0/aioclock/triggers.py
+-rw-r--r--   0        0        0     1042 2024-05-23 20:18:50.277093 aioclock-0.1.0/aioclock/types.py
+-rw-r--r--   0        0        0      862 2024-05-23 20:18:50.277093 aioclock-0.1.0/aioclock/utils.py
+-rw-r--r--   0        0        0     2139 2024-05-23 20:19:12.429257 aioclock-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4303 1970-01-01 00:00:00.000000 aioclock-0.1.0/PKG-INFO
```

### Comparing `aioclock-0.0.7/LICENSE` & `aioclock-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aioclock-0.0.7/README.md` & `aioclock-0.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 - **Github repository**: <https://github.com/ManiMozaffar/aioclock/>
 
 ## Features
 
 Aioclock offers:
 
 - Async: 100% Async, very light, fast and resource friendly
-- Scheduling: Keep scheduling tasks for yoo
+- Scheduling: Keep scheduling tasks for you
 - Group: Group your task, for better code maintainability
 - Trigger: Already defined and easily extendable triggers, to trigger your scheduler to be started
 - Easy syntax: Library's syntax is very easy and enjoyable, no confusing hierarchy
 - Pydantic v2 validation: Validate all your trigger on startup using pydantic 2. Fastest to fail possible!
 - **Soon**: Running the task dispatcher (scheduler) on different process by default, so CPU intensive stuff on task won't delay the scheduling
 - **Soon**: Backend support, to allow horizontal scalling, by synchronizing, maybe using Redis
```

### Comparing `aioclock-0.0.7/aioclock/app.py` & `aioclock-0.1.0/aioclock/app.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,61 @@
+"""
+To initialize the AioClock instance, you need to import the AioClock class from the aioclock module.
+AioClock class represent the aioclock, and handle the tasks and groups that will be run by the aioclock.
+
+Another way to modulize your code is to use `Group` which is kinda the same idea as router in web frameworks.
+"""
+
 import asyncio
+import sys
 from functools import wraps
-from typing import Any, Callable
+from typing import Any, Awaitable, Callable, TypeVar, Union
+
+if sys.version_info < (3, 10):
+    from typing_extensions import ParamSpec
+else:
+    from typing import ParamSpec
 
 from fast_depends import inject
 
 from aioclock.group import Group, Task
 from aioclock.provider import get_provider
 from aioclock.triggers import BaseTrigger
 from aioclock.types import Triggers
 from aioclock.utils import flatten_chain
 
+T = TypeVar("T")
+P = ParamSpec("P")
+
 
 class AioClock:
     """
     AioClock is the main class that will be used to run the tasks.
     It will be responsible for running the tasks in the right order.
 
     Example:
 
-    ```python
-    from aioclock import AioClock, Once
-    app = AioClock()
-
-    @app.task(trigger=Once())
-    async def main():
-        print("Hello World")
-    ```
+        ```python
+        from aioclock import AioClock, Once
+        app = AioClock()
+
+        @app.task(trigger=Once())
+        async def main():
+            print("Hello World")
+        ```
 
     To run the aioclock final app simply do:
 
-    ```python
-    from aioclock import AioClock, Once
-    app = AioClock()
-
-    # whatever next comes here
-    await app.serve()
-    ```
+        ```python
+        from aioclock import AioClock, Once
+        app = AioClock()
+
+        # whatever next comes here
+        await app.serve()
+        ```
 
     """
 
     def __init__(self):
         """
         Initialize AioClock instance.
         No parameters are needed.
@@ -60,70 +76,69 @@
 
     def override_dependencies(
         self, original: Callable[..., Any], override: Callable[..., Any]
     ) -> None:
         """Override a dependency with a new one.
 
         Example:
+            ```python
+            from aioclock import AioClock
 
-        ```python
-        from aioclock import AioClock
-
-        def original_dependency():
-            return 1
+            def original_dependency():
+                return 1
 
-        def new_dependency():
-            return 2
+            def new_dependency():
+                return 2
 
-        app = AioClock()
-        app.override_dependencies(original=original_dependency, override=new_dependency)
-        ```
+            app = AioClock()
+            app.override_dependencies(original=original_dependency, override=new_dependency)
+            ```
 
         """
         self.dependencies.override(original, override)
 
     def include_group(self, group: Group) -> None:
         """Include a group of tasks that will be run by AioClock.
-        Example:
 
-        ```python
-        from aioclock import AioClock, Group, Once
+        Example:
+            ```python
+            from aioclock import AioClock, Group, Once
 
-        app = AioClock()
+            app = AioClock()
 
-        group = Group()
-        @group.task(trigger=Once())
-        async def main():
-            print("Hello World")
+            group = Group()
+            @group.task(trigger=Once())
+            async def main():
+                print("Hello World")
 
-        app.include_group(group)
-        ```
+            app.include_group(group)
+            ```
         """
         self._groups.append(group)
         return None
 
     def task(self, *, trigger: BaseTrigger):
         """Decorator to add a task to the AioClock instance.
 
         Example:
 
-        ```python
-        from aioclock import AioClock, Once
+            ```python
+            from aioclock import AioClock, Once
 
-        app = AioClock()
+            app = AioClock()
 
-        @app.task(trigger=Once())
-        async def main():
-            print("Hello World")
-        ```
+            @app.task(trigger=Once())
+            async def main():
+                print("Hello World")
+            ```
         """
 
-        def decorator(func: Callable[..., Any]) -> Callable[..., Any]:
+        def decorator(func: Callable[P, Awaitable[T]]) -> Callable[P, Awaitable[T]]:
             @wraps(func)
-            async def wrapper(*args, **kwargs) -> Any:
+            async def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
                 return await func(*args, **kwargs)
 
             self._app_tasks.append(
                 Task(
                     func=inject(wrapper, dependency_overrides_provider=get_provider()),
                     trigger=trigger,
                 )
@@ -139,20 +154,22 @@
 
     def _get_shutdown_task(self) -> list[Task]:
         return [task for task in self._tasks if task.trigger.type_ == Triggers.ON_SHUT_DOWN]
 
     def _get_startup_task(self) -> list[Task]:
         return [task for task in self._tasks if task.trigger.type_ == Triggers.ON_START_UP]
 
-    def _get_tasks(self) -> list[Task]:
-        return [
-            task
-            for task in self._tasks
-            if task.trigger.type_ not in {Triggers.ON_START_UP, Triggers.ON_SHUT_DOWN}
-        ]
+    def _get_tasks(self, exclude_type: Union[set[Triggers], None] = None) -> list[Task]:
+        exclude_type = (
+            exclude_type
+            if exclude_type is not None
+            else {Triggers.ON_START_UP, Triggers.ON_SHUT_DOWN}
+        )
+
+        return [task for task in self._tasks if task.trigger.type_ not in exclude_type]
 
     async def serve(self) -> None:
         """
         Serves AioClock
         Run the tasks in the right order.
         First, run the startup tasks, then run the tasks, and finally run the shutdown tasks.
         """
```

### Comparing `aioclock-0.0.7/aioclock/triggers.py` & `aioclock-0.1.0/aioclock/triggers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,29 @@
+"""
+Triggers are used to determine when the event should be triggered. It can be based on time, or some other condition.
+You can create custom triggers by inheriting from `BaseTrigger` class.
+
+!!! info "Don't run CPU intensitve or thread-block IO task "
+    AioClock's trigger are all running in async, only on one CPU.
+    So, if you run a CPU intensive task, or a task that blocks the thread, then it will block the entire event loop.
+    If you have a sync IO task, then it's recommended to use `run_in_executor` to run the task in a separate thread.
+    Or use similiar libraries like `asyncer` or `trio` to run the task in a separate thread.
+"""
+
 import asyncio
 from abc import ABC, abstractmethod
 from copy import deepcopy
 from datetime import datetime, timedelta
-from typing import Generic, Literal, TypeVar, Union
+from typing import Annotated, Generic, Literal, TypeVar, Union
 
 import zoneinfo
-from pydantic import BaseModel, PositiveInt, model_validator
+from annotated_types import Interval
+from pydantic import BaseModel, Field, PositiveInt, model_validator
 
-from aioclock.types import EveryT, HourT, MinuteT, PositiveNumber, SecondT, Triggers
+from aioclock.types import EveryT, PositiveNumber, Triggers
 
 TriggerTypeT = TypeVar("TriggerTypeT")
 
 
 class BaseTrigger(BaseModel, ABC, Generic[TriggerTypeT]):
     """
     Base class for all triggers.
@@ -20,41 +32,43 @@
 
     The way trigger are used is as follows:
         1. An async function which is a task, is decorated with framework, and trigger is the arguement for the decorator
         2. `get_waiting_time_till_next_trigger` is called to get the time in seconds, after which the event should be triggered.
         3. If the time is not None, then it logs the time that is predicted for the event to be triggered.
         4. `trigger_next` is called immidiately after that, which triggers the event.
 
-    This is an example to implement a custom trigger, by yourself:
+    You can create trigger by yourself, by inheriting from `BaseTrigger` class.
 
-    ```python
-    from aioclock.triggers import BaseTrigger
+    Example:
+        ```python
+        from aioclock.triggers import BaseTrigger
 
 
-    class Forever(BaseTrigger[Literal["Forever"]]):
-        type_: Literal["Forever"] = "Forever"
+        class Forever(BaseTrigger[Literal["Forever"]]):
+            type_: Literal["Forever"] = "Forever"
 
-        def should_trigger(self) -> bool:
-            return True
+            def should_trigger(self) -> bool:
+                return True
 
-        async def trigger_next(self) -> None:
-            return None
+            async def trigger_next(self) -> None:
+                return None
 
-        async def get_waiting_time_till_next_trigger(self):
-            if self.should_trigger():
-                return 0
-            return None
-    ```
+            async def get_waiting_time_till_next_trigger(self):
+                if self.should_trigger():
+                    return 0
+                return None
+        ```
+
+    Attributes:
+        type_: Type of the trigger. It is a string, which is used to identify the trigger's name.
+            You can change the type by using `Generic` type when inheriting from `BaseTrigger`.
     """
 
     type_: TriggerTypeT
-    """
-    Type of the trigger. It is a string, which is used to identify the trigger's name.
-    You can change the type by using `Generic` type when inheriting from `BaseTrigger`.
-    """
+    expected_trigger_time: Union[datetime, None] = None
 
     @abstractmethod
     async def trigger_next(self) -> None:
         """
         `trigger_next` keep track of the event, and triggers the event.
         The function shall return when the event is triggered and should be executed.
         """
@@ -78,35 +92,40 @@
         ...
 
 
 class Forever(BaseTrigger[Literal[Triggers.FOREVER]]):
     """A trigger that is always triggered imidiately.
 
     Example:
-    ```python
+        ```python
 
-        from aioclock import AioClock,
+            from aioclock import AioClock,
 
-        app = AioClock()
+            app = AioClock()
+
+            # instead of this:
+            async def my_task():
+                while True:
+                    try:
+                        await asyncio.sleep(3)
+                        1/0
+                    excpet DivisionByZero:
+                        pass
+
+            # use this:
+            @app.task(trigger=Forever())
+            async def my_task():
+                await asyncio.sleep(3)
+                1/0
+        ```
+
+    Attributes:
+        type_: Type of the trigger. It is a string, which is used to identify the trigger's name.
+            You can change the type by using `Generic` type when inheriting from `BaseTrigger`.
 
-        # instead of this:
-        async def my_task():
-            while True:
-                try:
-                    await asyncio.sleep(3)
-                    1/0
-                excpet DivisionByZero:
-                    pass
-
-        # use this:
-        @app.task(trigger=Forever())
-        async def my_task():
-            await asyncio.sleep(3)
-            1/0
-    ```
     """
 
     type_: Literal[Triggers.FOREVER] = Triggers.FOREVER
 
     def should_trigger(self) -> bool:
         return True
 
@@ -116,47 +135,41 @@
     async def get_waiting_time_till_next_trigger(self):
         return 0
 
 
 class LoopController(BaseTrigger, ABC, Generic[TriggerTypeT]):
     """
     Base class for all triggers that have loop control.
-    """
 
-    type_: TriggerTypeT
-    """
-    Type of the trigger. It is a string, which is used to identify the trigger's name.
-    You can change the type by using `Generic` type when inheriting from `BaseTrigger`.
+    Attributes:
+        type_: Type of the trigger. It is a string, which is used to identify the trigger's name.
+            You can change the type by using `Generic` type when inheriting from `LoopController`.
+
+        max_loop_count: The maximum number of times the event should be triggered.
+            If set to 3, then 4th time the event will not be triggered.
+            If set to None, it will keep running forever.
+            This is available for all triggers that inherit from `LoopController`.
+
+        _current_loop_count: Current loop count, which is used to keep track of the number of times the event has been triggered.
+            Private attribute, should not be accessed directly.
+            This is available for all triggers that inherit from `LoopController`.
     """
 
+    type_: TriggerTypeT
     _current_loop_count: int = 0
-    """
-    Current loop count, which is used to keep track of the number of times the event has been triggered.
-    Private attribute, should not be accessed directly.
-    """
-
     max_loop_count: Union[PositiveInt, None] = None
-    """
-    The maximum number of times the event should be triggered.
-
-    If set to 3, then 4th time the event will not be triggered.
-    If set to None, it will keep running forever.
-
-    This is available for all triggers that inherit from `LoopController`.
-    """
 
     @model_validator(mode="after")
     def validate_loop_controll(self):
         if "_current_loop_count" in self.model_fields_set:
             raise ValueError("_current_loop_count is a private attribute, should not be provided.")
         return self
 
     def _increment_loop_counter(self) -> None:
-        if self._current_loop_count is not None:
-            self._current_loop_count += 1
+        self._current_loop_count += 1
 
     def should_trigger(self) -> bool:
         if self.max_loop_count is None:
             return True
         if self._current_loop_count < self.max_loop_count:
             return True
         return False
@@ -165,120 +178,133 @@
         return 0
 
 
 class Once(LoopController[Literal[Triggers.ONCE]]):
     """A trigger that is triggered only once. It is used to trigger the event only once, and then stop.
 
     Example:
-    ```python
-    from aioclock import AioClock, Once
-    app = AioClock()
-
-    app.task(trigger=Once())
-    async def task():
-        print("Hello World!")
-    ```
+        ```python
+        from aioclock import AioClock, Once
+        app = AioClock()
+
+        app.task(trigger=Once())
+        async def task():
+            print("Hello World!")
+        ```
+
+    Attributes:
+        max_loop_count: The maximum number of times the event should be triggered. Should be always 1 for this trigger.
     """
 
     type_: Literal[Triggers.ONCE] = Triggers.ONCE
-    max_loop_count: PositiveInt = 1
-    """The maximum number of times the event should be triggered. Should be always 1 for this trigger"""
+    max_loop_count: Literal[1] = 1
 
     async def trigger_next(self) -> None:
         self._increment_loop_counter()
         return None
 
     async def get_waiting_time_till_next_trigger(self):
-        return 0
+        if self._current_loop_count == 0:
+            return 0
+        return None
 
 
 class OnStartUp(LoopController[Literal[Triggers.ON_START_UP]]):
     """Just like Once, but it triggers the event only once, when the application starts up.
 
     Example:
-    ```python
-    from aioclock import AioClock, OnStartUp
-    app = AioClock()
-
-    app.task(trigger=OnStartUp())
-    async def task():
-        print("Hello World!")
-    ```
+        ```python
+        from aioclock import AioClock, OnStartUp
+        app = AioClock()
+
+        app.task(trigger=OnStartUp())
+        async def task():
+            print("Hello World!")
+        ```
+
+    Attributes:
+        max_loop_count: The maximum number of times the event should be triggered. Should be always 1 for this trigger.
     """
 
     type_: Literal[Triggers.ON_START_UP] = Triggers.ON_START_UP
-    max_loop_count: PositiveInt = 1
-    """The maximum number of times the event should be triggered. Should be always 1 for this trigger."""
+    max_loop_count: Literal[1] = 1
 
     async def trigger_next(self) -> None:
         self._increment_loop_counter()
         return None
 
     async def get_waiting_time_till_next_trigger(self):
-        return 0
+        if self._current_loop_count == 0:
+            return 0
+        return None
 
 
 class OnShutDown(LoopController[Literal[Triggers.ON_SHUT_DOWN]]):
     """Just like Once, but it triggers the event only once, when the application shuts down.
 
     Example:
-    ```python
-    from aioclock import AioClock, OnShutDown
-    app = AioClock()
-
-    app.task(trigger=OnShutDown())
-    async def task():
-        print("Hello World!")
-    ```
+        ```python
+        from aioclock import AioClock, OnShutDown
+        app = AioClock()
+
+        app.task(trigger=OnShutDown())
+        async def task():
+            print("Hello World!")
+        ```
 
+    Attributes:
+        max_loop_count: The maximum number of times the event should be triggered. Should be always 1 for this trigger.
     """
 
     type_: Literal[Triggers.ON_SHUT_DOWN] = Triggers.ON_SHUT_DOWN
-    max_loop_count: PositiveInt = 1
-    """The maximum number of times the event should be triggered. Should be always 1 for this trigger."""
+    max_loop_count: Literal[1] = 1
 
     async def trigger_next(self) -> None:
         self._increment_loop_counter()
         return None
 
     async def get_waiting_time_till_next_trigger(self):
-        return 0
+        if self._current_loop_count == 0:
+            return 0
+        return None
 
 
 class Every(LoopController[Literal[Triggers.EVERY]]):
     """A trigger that is triggered every x time units.
 
     Example:
-    ```python
-    from aioclock import AioClock, Every
-    app = AioClock()
-
-    app.task(trigger=Every(seconds=3))
-    async def task():
-        print("Hello World!")
-    ```
+        ```python
+        from aioclock import AioClock, Every
+        app = AioClock()
 
+        app.task(trigger=Every(seconds=3))
+        async def task():
+            print("Hello World!")
+        ```
+
+    Attributes:
+        first_run_strategy: Strategy to use for the first run.
+            If `immediate`, then the event will be triggered immediately,
+                and then wait for the time to trigger the event again.
+            If `wait`, then the event will wait for the time to trigger the event for the first time.
+
+        seconds: Seconds to wait before triggering the event.
+        minutes: Minutes to wait before triggering the event.
+        hours: Hours to wait before triggering the event.
+        days: Days to wait before triggering the event.
+        weeks: Weeks to wait before triggering the event.
     """
 
     type_: Literal[Triggers.EVERY] = Triggers.EVERY
-
+    first_run_strategy: Literal["immediate", "wait"] = "wait"
     seconds: Union[PositiveNumber, None] = None
-    """Seconds to wait before triggering the event."""
-
     minutes: Union[PositiveNumber, None] = None
-    """Minutes to wait before triggering the event."""
-
     hours: Union[PositiveNumber, None] = None
-    """Hours to wait before triggering the event."""
-
     days: Union[PositiveNumber, None] = None
-    """Days to wait before triggering the event."""
-
     weeks: Union[PositiveNumber, None] = None
-    """Weeks to wait before triggering the event."""
 
     @model_validator(mode="after")
     def validate_time_units(self):
         if (
             self.seconds is None
             and self.minutes is None
             and self.hours is None
@@ -301,59 +327,72 @@
         if self.minutes is not None:
             result += self.minutes * 60
 
         return result
 
     async def trigger_next(self) -> None:
         self._increment_loop_counter()
+        if self._current_loop_count == 1 and self.first_run_strategy == "immediate":
+            return None
         await asyncio.sleep(self.to_seconds)
-        return
+        return None
 
     async def get_waiting_time_till_next_trigger(self):
+        # not incremented yet, so the counter is 0
+        if self._current_loop_count == 0 and self.first_run_strategy == "immediate":
+            return 0
+
         if self.should_trigger():
             return self.to_seconds
         return None
 
 
 WEEK_TO_SECOND = 604800
 
 
 class At(LoopController[Literal[Triggers.AT]]):
     """A trigger that is triggered at a specific time.
 
     Example:
-    ```python
+        ```python
 
-    from aioclock import AioClock, At
+        from aioclock import AioClock, At
 
-    app = AioClock()
+        app = AioClock()
+
+        @app.task(trigger=At(hour=12, minute=30, tz="Asia/Kolkata"))
+        async def task():
+            print("Hello World!")
+        ```
+
+    Attributes:
+        second: Second to trigger the event.
+        minute: Minute to trigger the event.
+        hour: Hour to trigger the event.
+        at: Day of week to trigger the event. You would get the in-line typing support when using the trigger.
+        tz: Timezone to use for the event.
 
-    @app.task(trigger=At(hour=12, minute=30, tz="Asia/Kolkata"))
-    async def task():
-        print("Hello World!")
-    ```
     """
 
     type_: Literal[Triggers.AT] = Triggers.AT
 
-    second: SecondT = 0
-    """Second to trigger the event."""
-
-    minute: MinuteT = 0
-    """Minute to trigger the event."""
-
-    hour: HourT = 0
-    """Hour to trigger the event."""
-
-    at: EveryT = "every day"
-    """Day of week to trigger the event. You would get the in-line typing support when using the trigger.
-    """
-
+    second: Annotated[int, Interval(ge=0, le=59)] = 0
+    minute: Annotated[int, Interval(ge=0, le=59)] = 0
+    hour: Annotated[int, Interval(ge=0, le=24)] = 0
+    at: Literal[
+        "every monday",
+        "every tuesday",
+        "every wednesday",
+        "every thursday",
+        "every friday",
+        "every saturday",
+        "every sunday",
+        "every day",
+    ] = "every day"
     tz: str
-    """Timzeon to use for the event."""
 
     @model_validator(mode="after")
     def validate_time_units(self):
         if self.second is None and self.minute is None and self.hour is None:
             raise ValueError("At least one time unit must be provided.")
 
         if self.tz is not None:
@@ -411,7 +450,12 @@
 
     async def get_waiting_time_till_next_trigger(self):
         return self.get_sleep_time()
 
     async def trigger_next(self) -> None:
         self._increment_loop_counter()
         await asyncio.sleep(self.get_sleep_time())
+
+
+TriggerT = Annotated[
+    Union[Forever, Once, Every, At, OnStartUp, OnShutDown], Field(discriminator="type_")
+]
```

### Comparing `aioclock-0.0.7/aioclock/types.py` & `aioclock-0.1.0/aioclock/types.py`

 * *Files identical despite different names*

### Comparing `aioclock-0.0.7/aioclock/utils.py` & `aioclock-0.1.0/aioclock/utils.py`

 * *Files identical despite different names*

### Comparing `aioclock-0.0.7/pyproject.toml` & `aioclock-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 [tool.poetry]
 name = "aioclock"
-version = "0.0.7"
+version = "0.1.0"
 description = "An asyncio-based scheduling framework designed for execution of periodic task with integrated support for dependency injection, enabling efficient and flexiable task management"
 authors = ["Mani Mozaffar <fmani.mozaffar@gmail.com>"]
 repository = "https://github.com/ManiMozaffar/aioclock"
 documentation = "https://ManiMozaffar.github.io/aioclock/"
 readme = "README.md"
 packages = [{ include = "aioclock" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 pydantic = "^2.6.4"
 fast-depends = "^2.4.2"
+pytest-asyncio = "^0.23.7"
+
+[tool.poetry.group.extras.dependencies]
+fastapi = { version = ">0.90.0", extras = ["fastapi"] }
+
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-asyncio = "^0.23.6"
 tox = "^4.11.1"
 rich = "^13.7.1"
 pyright = "1.1.350"
```

### Comparing `aioclock-0.0.7/PKG-INFO` & `aioclock-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: aioclock
-Version: 0.0.7
+Version: 0.1.0
 Summary: An asyncio-based scheduling framework designed for execution of periodic task with integrated support for dependency injection, enabling efficient and flexiable task management
 Home-page: https://github.com/ManiMozaffar/aioclock
 Author: Mani Mozaffar
 Author-email: fmani.mozaffar@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: fast-depends (>=2.4.2,<3.0.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
+Requires-Dist: pytest-asyncio (>=0.23.7,<0.24.0)
 Project-URL: Documentation, https://ManiMozaffar.github.io/aioclock/
 Project-URL: Repository, https://github.com/ManiMozaffar/aioclock
 Description-Content-Type: text/markdown
 
 # aioclock
 
 [![Release](https://img.shields.io/github/v/release/ManiMozaffar/aioclock)](https://img.shields.io/github/v/release/ManiMozaffar/aioclock)
@@ -30,15 +31,15 @@
 - **Github repository**: <https://github.com/ManiMozaffar/aioclock/>
 
 ## Features
 
 Aioclock offers:
 
 - Async: 100% Async, very light, fast and resource friendly
-- Scheduling: Keep scheduling tasks for yoo
+- Scheduling: Keep scheduling tasks for you
 - Group: Group your task, for better code maintainability
 - Trigger: Already defined and easily extendable triggers, to trigger your scheduler to be started
 - Easy syntax: Library's syntax is very easy and enjoyable, no confusing hierarchy
 - Pydantic v2 validation: Validate all your trigger on startup using pydantic 2. Fastest to fail possible!
 - **Soon**: Running the task dispatcher (scheduler) on different process by default, so CPU intensive stuff on task won't delay the scheduling
 - **Soon**: Backend support, to allow horizontal scalling, by synchronizing, maybe using Redis
```

