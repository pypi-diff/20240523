# Comparing `tmp/django-compositepk-model-1.0.2.tar.gz` & `tmp/django_compositepk_model-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\sakur\source\repos\Package\django-compositepk-model\dist\tmp8v818qxr\django-compositepk-model-1.0.2.tar", last modified: Sat Mar 13 04:03:08 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `django-compositepk-model-1.0.2.tar` & `django_compositepk_model-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,10 @@
-drwxrwxrwx   0        0        0        0 2021-03-13 04:03:08.000000 django-compositepk-model-1.0.2/
--rw-rw-rw-   0        0        0     4750 2021-03-13 04:03:08.000000 django-compositepk-model-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3333 2021-03-13 03:23:59.000000 django-compositepk-model-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2021-03-13 04:03:07.000000 django-compositepk-model-1.0.2/cpkmodel/
--rw-rw-rw-   0        0        0      302 2021-01-29 06:03:23.000000 django-compositepk-model-1.0.2/cpkmodel/__init__.py
--rw-rw-rw-   0        0        0     1288 2021-01-30 00:47:52.000000 django-compositepk-model-1.0.2/cpkmodel/compositekey.py
--rw-rw-rw-   0        0        0      160 2021-01-29 06:03:23.000000 django-compositepk-model-1.0.2/cpkmodel/constants.py
--rw-rw-rw-   0        0        0     4622 2021-03-13 02:52:40.000000 django-compositepk-model-1.0.2/cpkmodel/cpkmodel.py
--rw-rw-rw-   0        0        0     9724 2021-03-13 02:52:40.000000 django-compositepk-model-1.0.2/cpkmodel/cpkquery.py
-drwxrwxrwx   0        0        0        0 2021-03-13 04:03:08.000000 django-compositepk-model-1.0.2/django_compositepk_model.egg-info/
--rw-rw-rw-   0        0        0     4750 2021-03-13 04:03:07.000000 django-compositepk-model-1.0.2/django_compositepk_model.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2021-03-13 04:03:07.000000 django-compositepk-model-1.0.2/django_compositepk_model.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-03-13 04:03:07.000000 django-compositepk-model-1.0.2/django_compositepk_model.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2021-03-13 04:03:07.000000 django-compositepk-model-1.0.2/django_compositepk_model.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-03-13 04:03:08.000000 django-compositepk-model-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      892 2021-03-13 03:28:19.000000 django-compositepk-model-1.0.2/setup.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 django_compositepk_model-1.0.3/compositepk-model/cpkmodel/__init__.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 django_compositepk_model-1.0.3/compositepk-model/cpkmodel/compositekey.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 django_compositepk_model-1.0.3/compositepk-model/cpkmodel/constants.py
+-rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 django_compositepk_model-1.0.3/compositepk-model/cpkmodel/cpkmodel.py
+-rw-r--r--   0        0        0     9419 2020-02-02 00:00:00.000000 django_compositepk_model-1.0.3/compositepk-model/cpkmodel/cpkquery.py
+-rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 django_compositepk_model-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 django_compositepk_model-1.0.3/LICENSE
+-rw-r--r--   0        0        0     4904 2020-02-02 00:00:00.000000 django_compositepk_model-1.0.3/README.md
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 django_compositepk_model-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 django_compositepk_model-1.0.3/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-compositepk-model-1.0.2/cpkmodel/cpkmodel.py` & `django_compositepk_model-1.0.3/compositepk-model/cpkmodel/cpkmodel.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-from django.db import router
-from django.db.models import Model
-from django.db.models.base import ModelBase
-from django.db.models.deletion import Collector
-
-from .constants import CPK_SEP
-from .compositekey import CompositeKey
-from .cpkquery import CPkQuerySet
-
-
-class CompositePk(CompositeKey):
-    def __init__(self, keys):
-        super().__init__(keys, primary=True)
-        
-
-class CPkModelMixin:
-    @property
-    def pkvals(self):
-        return tuple(getattr(self, key.attname) for key in self.pkeys)
-
-    def _get_cpk_val(self, meta=None):
-        meta = meta or self._meta
-        key_values = getattr(self, 'pkvals')
-        if key_values:
-            if None in key_values:
-                return None
-            else:
-                strvalues = tuple((str(val) for val in key_values))
-                value = CPK_SEP.join(strvalues)
-                # MEMO: record for admin
-                setattr(self, meta.pk.attname, value)
-                return value
-        else:
-            return None
-
-    def _set_cpk_val(self, value):
-        super()._set_pk_val(value)
-        # set into original filelds
-        meta = self._meta
-        vals = value.split(CPK_SEP)
-        for key, val in zip(self.pkeys, vals):
-            setattr(self, key.attname, val)
-
-    cpk = property(_get_cpk_val, _set_cpk_val)
-
-    @staticmethod
-    def _no_check():
-        return []
-
-    def get_pk_lookups(self):
-        if self.has_compositepk:
-            keys = self.pkeys
-            vals = self.pkvals
-            return { key.attname:val for key, val in zip(keys, vals)}
-        else:
-            return { 'pk':self.pk }
-        
-
-    ###########################
-    # override
-    ###########################
-    def delete(self, using=None, keep_parents=False):
-        using = using or router.db_for_write(self.__class__, instance=self)
-        assert self.pk is not None, (
-            "%s object can't be deleted because its %s attribute is set to None." %
-            (self._meta.object_name, self._meta.pk.attname)
-        )
-
-        collector = Collector(using=using)
-        # Change S
-        #   MEMO: Collector doesn't support method to change its base query.
-        #           Therefore, I changed param '[self]' to CPkQuerySet object.
-        #
-        #collector.collect([self], keep_parents=keep_parents)
-        model = self._meta.model
-        qs = model.objects.filter(pk=self.pk)
-        collector.collect(qs, keep_parents=keep_parents)
-        # Change E
-        return collector.delete()
-
-
-class CPkModelBase(ModelBase):
-    """ Metaclass for CompositePkModel."""
-    def __new__(cls, name, bases, attrs, **kwargs):
-        if name == 'CPkModel':
-            # change bsses=(), because don't wanto to add app_talbe, CompositePkModel is only "Intermediate"
-            return super().__new__(cls, name, (), attrs, **kwargs) 
-        else:
-            modelbases = []
-            IntermediateClass = globals()['CPkModel']
-            for base in bases:
-                if base == IntermediateClass:
-                    # skip "Intermediate" CPkModel and change to Model
-                    modelbases.append(Model)
-                else:
-                    modelbases.append(base)
-            super_new = super().__new__(cls, name, tuple(modelbases), attrs, **kwargs)
-            meta = super_new._meta
-            pkeys = tuple(f for f in meta.local_concrete_fields if f.primary_key)
-            # change attributes
-            if len(pkeys) > 1:
-                super_new.has_compositepk = True
-                meta.pk = CompositePk(pkeys)
-                setattr(super_new, "pk", CPkModelMixin.cpk)
-                setattr(super_new, "_get_pk_val", CPkModelMixin._get_cpk_val)
-                setattr(super_new, "_set_pk_val", CPkModelMixin._set_cpk_val)
-                setattr(super_new, meta.pk.attname, None)
-                setattr(super_new, "_check_single_primary_key", CPkModelMixin._no_check)
-                setattr(super_new, "delete", CPkModelMixin.delete)
-            else:
-                super_new.has_compositepk = False
-            setattr(super_new, "get_pk_lookups", CPkModelMixin.get_pk_lookups)
-            meta.base_manager._queryset_class = CPkQuerySet
-            meta.default_manager._queryset_class = CPkQuerySet           
-            super_new.pkeys = pkeys
-            super_new.pkvals = CPkModelMixin.pkvals
-            super_new._meta = meta
-            return super_new
-
-
-class CPkModel(CPkModelMixin, Model, metaclass=CPkModelBase):
-    pass
+from django.db import router
+from django.db.models import Model
+from django.db.models.base import ModelBase
+from django.db.models.deletion import Collector
+
+from .constants import CPK_SEP
+from .compositekey import CompositeKey
+from .cpkquery import CPkQuerySet
+
+
+class CompositePk(CompositeKey):
+    def __init__(self, keys):
+        super().__init__(keys, primary=True)
+        
+
+class CPkModelMixin:
+    @property
+    def pkvals(self):
+        return tuple(getattr(self, key.attname) for key in self.pkeys)
+
+    def _get_cpk_val(self, meta=None):
+        meta = meta or self._meta
+        key_values = getattr(self, 'pkvals')
+        if key_values:
+            if None in key_values:
+                return None
+            else:
+                strvalues = tuple((str(val) for val in key_values))
+                value = CPK_SEP.join(strvalues)
+                # MEMO: record for admin
+                setattr(self, meta.pk.attname, value)
+                return value
+        else:
+            return None
+
+    def _set_cpk_val(self, value):
+        super()._set_pk_val(value)
+        # set into original filelds
+        meta = self._meta
+        vals = value.split(CPK_SEP)
+        for key, val in zip(self.pkeys, vals):
+            setattr(self, key.attname, val)
+
+    cpk = property(_get_cpk_val, _set_cpk_val)
+
+    @staticmethod
+    def _no_check():
+        return []
+
+    def get_pk_lookups(self):
+        if self.has_compositepk:
+            keys = self.pkeys
+            vals = self.pkvals
+            return { key.attname:val for key, val in zip(keys, vals)}
+        else:
+            return { 'pk':self.pk }
+        
+
+    ###########################
+    # override
+    ###########################
+    def delete(self, using=None, keep_parents=False):
+        using = using or router.db_for_write(self.__class__, instance=self)
+        assert self.pk is not None, (
+            "%s object can't be deleted because its %s attribute is set to None." %
+            (self._meta.object_name, self._meta.pk.attname)
+        )
+
+        collector = Collector(using=using)
+        # Change S
+        #   MEMO: Collector doesn't support method to change its base query.
+        #           Therefore, I changed param '[self]' to CPkQuerySet object.
+        #
+        #collector.collect([self], keep_parents=keep_parents)
+        model = self._meta.model
+        qs = model.objects.filter(pk=self.pk)
+        collector.collect(qs, keep_parents=keep_parents)
+        # Change E
+        return collector.delete()
+
+
+class CPkModelBase(ModelBase):
+    """ Metaclass for CompositePkModel."""
+    def __new__(cls, name, bases, attrs, **kwargs):
+        if name == 'CPkModel':
+            # change bsses=(), because don't wanto to add app_talbe, CompositePkModel is only "Intermediate"
+            return super().__new__(cls, name, (), attrs, **kwargs) 
+        else:
+            modelbases = []
+            IntermediateClass = globals()['CPkModel']
+            for base in bases:
+                if base == IntermediateClass:
+                    # skip "Intermediate" CPkModel and change to Model
+                    modelbases.append(Model)
+                else:
+                    modelbases.append(base)
+            super_new = super().__new__(cls, name, tuple(modelbases), attrs, **kwargs)
+            meta = super_new._meta
+            pkeys = tuple(f for f in meta.local_concrete_fields if f.primary_key)
+            # change attributes
+            if len(pkeys) > 1:
+                super_new.has_compositepk = True
+                meta.pk = CompositePk(pkeys)
+                setattr(super_new, "pk", CPkModelMixin.cpk)
+                setattr(super_new, "_get_pk_val", CPkModelMixin._get_cpk_val)
+                setattr(super_new, "_set_pk_val", CPkModelMixin._set_cpk_val)
+                setattr(super_new, meta.pk.attname, None)
+                setattr(super_new, "_check_single_primary_key", CPkModelMixin._no_check)
+                setattr(super_new, "delete", CPkModelMixin.delete)
+            else:
+                super_new.has_compositepk = False
+            setattr(super_new, "get_pk_lookups", CPkModelMixin.get_pk_lookups)
+            meta.base_manager._queryset_class = CPkQuerySet
+            meta.default_manager._queryset_class = CPkQuerySet           
+            super_new.pkeys = pkeys
+            super_new.pkvals = CPkModelMixin.pkvals
+            super_new._meta = meta
+            return super_new
+
+
+class CPkModel(CPkModelMixin, Model, metaclass=CPkModelBase):
+    pass
```

### Comparing `django-compositepk-model-1.0.2/cpkmodel/cpkquery.py` & `django_compositepk_model-1.0.3/compositepk-model/cpkmodel/cpkquery.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,223 +1,218 @@
-import copy
-
-from django.db import connections,transaction
-from django.db.models import QuerySet,Q
-from django.db.models.sql import Query, DeleteQuery, UpdateQuery
-from django.db.models.constants import LOOKUP_SEP
-from django.db.models.expressions import Case, Expression, Value, When
-from django.db.models.functions import Cast
-from django.db.utils import NotSupportedError,ProgrammingError
-
-from .constants import CPK_SEP
-from .compositekey import CompositeKey
-
-
-class CPkQueryMixin():
-    def _get_pk_names(self):
-        return tuple(key.name for key in self.model.pkeys)
-
-    ###########################
-    # override
-    ###########################
-
-    def chain(self, klass=None):
-        cpk_klass = klass
-        if klass == Query:
-            cpk_klass = CPkQuery
-        elif klass == UpdateQuery:
-            cpk_klass = CPkUpdateQuery
-        elif klass == DeleteQuery:
-            cpk_klass = CPkDeleteQuery
-
-        return super().chain(klass=cpk_klass)
-
-    def names_to_path(self, names, opts, allow_many=True, fail_on_missing=False):
-        meta = self.get_meta()
-        first_name = names[0]
-        # name[0] is Multi-Column ?
-        if (first_name == 'pk' and self.model.has_compositepk) or CPK_SEP in first_name:
-            # get CompisteKey
-            ckey = meta.pk
-            if first_name != 'pk' and first_name != ckey.name:
-                # IF Not PK, mnake another CompositeKey
-                cols = [meta.get_field(col) for col in first_name.split(CPK_SEP)]
-                ckey = CompositeKey(cols)
-            lookups = names[1:] if len(names) > 1 else []
-            return [], ckey, (ckey,), lookups
-        else:
-            return super().names_to_path(names, opts, allow_many, fail_on_missing)
-
-    def add_ordering(self, *ordering):
-        if 'pk' in ordering or '-pk' in ordering:
-            new_ordering = ()
-            for item in ordering:
-                if item == 'pk':
-                    new_ordering += self._get_pk_names()
-                elif item == '-pk':
-                    names = tuple('-' + name for name in self._get_pk_names())                    
-                    new_ordering += names
-                else:
-                    new_ordering += (item)
-            super().add_ordering(*new_ordering)
-        else:
-            super().add_ordering(*ordering)
-
-    def add_q(self, q_object):
-        def separate_key(self, key):
-            if key == 'pk':
-                return self._get_pk_names()
-            else:
-                return tuple(key.split(CPK_SEP))
-
-        def separate_value(keys, value):
-            if isinstance(value, str):
-                return tuple(value.split(CPK_SEP))
-            elif isinstance(value, tuple):
-                return value
-            elif isinstance(value, list):
-                return tuple(value)
-            elif isinstance(value, dict):
-                new_vals = tuple(value.get(key) for key in keys)
-                return new_vals
-            else:
-                return (value,)
-
-        def transform_q(obj):
-            def make_q(keys, vals):
-                q = Q()
-                for key, val in zip(keys, vals):
-                    q.children.append((key, val))
-                return q
-
-            assert isinstance(obj, (Q, tuple))
-            if isinstance(obj, Q):
-                # When obj is Q, transform children.
-                new_q = copy.copy(obj)
-                new_q.children = []
-                for child in obj.children:
-                    new_q.children.append(transform_q(child))
-                return new_q
-            else:
-                # When obj is tuple,
-                #  obj[0] is lhs(lookup expression)
-                #       pk and multi column with lookup 'in' is nothing to do in this, it will change in 'names_to_path'. 
-                #  obj[1] is rhs(values)
-                #       valeus are separated in this method.
-                names = obj[0].split(LOOKUP_SEP)
-                if ('pk' in names and self.model.has_compositepk) or CPK_SEP in obj[0]:
-                    # When composite-pk or multi-column
-                    if len(names) == 1:
-                        # change one Q to multi Q
-                        keys = separate_key(self, obj[0])
-                        vals = separate_value(keys, obj[1])
-                        if len(keys) == len(vals):
-                            return make_q(keys, vals)
-                        else:
-                            raise ProgrammingError("Parameter unmatch : key={} val={}".format(keys, vals))
-                    else:
-                        # check the last name
-                        last = names[-1]
-                        if last == 'in':
-                            if len(names) == 2:
-                                # for 'pk__in' or 'multi-column__in'
-                                keys = separate_key(self, names[-2])
-                                new_vals = [separate_value(keys, val) for val in obj[1]]
-                                return (obj[0], new_vals)
-                            elif CPK_SEP in names[-2]:
-                                # multi-column is not supported.
-                                raise NotSupportedError("Not supported multi-column with'in' on relation model : {}".format(obj[0]))
-                        elif last == 'pk' or CPK_SEP in last:
-                            # change one Q to multi Q
-                            #  example: ('relmodel__id1,id2', (valule1,value2))
-                            #             |
-                            #             V
-                            #           ('relmodel__id1', valule1)
-                            #           ('relmodel__id2', valule2)
-                            before_path = LOOKUP_SEP.join(names[0:-1])
-                            cols = separate_key(self, last)
-                            keys = [before_path +  LOOKUP_SEP + col for col in cols]
-                            vals = separate_value(cols, obj[1])
-                            return make_q(keys, vals)
-                        else:
-                            # another lookup is not supported.
-                            raise NotSupportedError("Not supported multi-column with '{}' : {}".format(last,obj[0]))
-                return obj
-
-        new_q = transform_q(q_object)
-        super().add_q(new_q)
-
-
-class CPkQuery(CPkQueryMixin, Query):
-    pass
-
-
-class CPkDeleteQuery(CPkQueryMixin, DeleteQuery):
-    pass
-
-
-class CPkUpdateQuery(CPkQueryMixin, UpdateQuery):
-    pass
-
-
-class CPkQuerySet(QuerySet):
-    ###########################
-    # override
-    ###########################
-
-    def __init__(self, model=None, query=None, using=None, hints=None):
-        if not query:
-            query = CPkQuery(model)
-        super().__init__(model, query, using, hints)
-
-    def bulk_update(self, objs, fields, batch_size=None):
-        """
-        Update the given fields in each of the given objects in the database.
-        """
-        if batch_size is not None and batch_size < 0:
-            raise ValueError('Batch size must be a positive integer.')
-        if not fields:
-            raise ValueError('Field names must be given to bulk_update().')
-        objs = tuple(objs)
-        if any(obj.pk is None for obj in objs):
-            raise ValueError('All bulk_update() objects must have a primary key set.')
-        fields = [self.model._meta.get_field(name) for name in fields]
-        if any(not f.concrete or f.many_to_many for f in fields):
-            raise ValueError('bulk_update() can only be used with concrete fields.')
-        if any(f.primary_key for f in fields):
-            raise ValueError('bulk_update() cannot be used with primary key fields.')
-        if not objs:
-            return
-        # PK is used twice in the resulting update query, once in the filter
-        # and once in the WHEN. Each field will also have one CAST.
-        max_batch_size = connections[self.db].ops.bulk_batch_size(['pk', 'pk'] + fields, objs)
-        batch_size = min(batch_size, max_batch_size) if batch_size else max_batch_size
-        requires_casting = connections[self.db].features.requires_casted_case_in_updates
-        batches = (objs[i:i + batch_size] for i in range(0, len(objs), batch_size))
-        updates = []
-        for batch_objs in batches:
-            update_kwargs = {}
-            for field in fields:
-                when_statements = []
-                for obj in batch_objs:
-                    attr = getattr(obj, field.attname)
-                    if not isinstance(attr, Expression):
-                        attr = Value(attr, output_field=field)
-                    # CHANGE S
-                    #when_statements.append(When(pk=obj.pk, then=attr))
-                    lookups = obj.get_pk_lookups()
-                    when_statements.append(When(**lookups, then=attr))
-                    # CHANGE E
-                case_statement = Case(*when_statements, output_field=field)
-                if requires_casting:
-                    case_statement = Cast(case_statement, output_field=field)
-                update_kwargs[field.attname] = case_statement
-            updates.append(([obj.pk for obj in batch_objs], update_kwargs))
-        with transaction.atomic(using=self.db, savepoint=False):
-            for pks, update_kwargs in updates:
-                self.filter(pk__in=pks).update(**update_kwargs)
-    bulk_update.alters_data = True
-
-    def _get_pk_condition(self, obj):
-        conditions = {}
-        
-        pass
+import copy
+
+from django.db import connections,transaction
+from django.db.models import QuerySet,Q
+from django.db.models.sql import Query, DeleteQuery, UpdateQuery
+from django.db.models.constants import LOOKUP_SEP
+from django.db.models.expressions import Case, Expression, Value, When
+from django.db.models.functions import Cast
+from django.db.utils import NotSupportedError,ProgrammingError
+
+from .constants import CPK_SEP
+from .compositekey import CompositeKey
+
+
+class CPkQueryMixin():
+    def _get_pk_names(self):
+        return tuple(key.name for key in self.model.pkeys)
+
+    ###########################
+    # override
+    ###########################
+
+    def chain(self, klass=None):
+        cpk_klass = klass
+        if klass == Query:
+            cpk_klass = CPkQuery
+        elif klass == UpdateQuery:
+            cpk_klass = CPkUpdateQuery
+        elif klass == DeleteQuery:
+            cpk_klass = CPkDeleteQuery
+
+        return super().chain(klass=cpk_klass)
+
+    def names_to_path(self, names, opts, allow_many=True, fail_on_missing=False):
+        meta = self.get_meta()
+        first_name = names[0]
+        # name[0] is Multi-Column ?
+        if (first_name == 'pk' and self.model.has_compositepk) or CPK_SEP in first_name:
+            # get CompisteKey
+            ckey = meta.pk
+            if first_name != 'pk' and first_name != ckey.name:
+                # IF Not PK, mnake another CompositeKey
+                cols = [meta.get_field(col) for col in first_name.split(CPK_SEP)]
+                ckey = CompositeKey(cols)
+            lookups = names[1:] if len(names) > 1 else []
+            return [], ckey, (ckey,), lookups
+        else:
+            return super().names_to_path(names, opts, allow_many, fail_on_missing)
+
+    def add_ordering(self, *ordering):
+        if 'pk' in ordering or '-pk' in ordering:
+            new_ordering = ()
+            for item in ordering:
+                if item == 'pk':
+                    new_ordering += self._get_pk_names()
+                elif item == '-pk':
+                    names = tuple('-' + name for name in self._get_pk_names())                    
+                    new_ordering += names
+                else:
+                    new_ordering += (item,)
+            super().add_ordering(*new_ordering)
+        else:
+            super().add_ordering(*ordering)
+
+    def add_q(self, q_object):
+        def separate_key(self, key):
+            if key == 'pk':
+                return self._get_pk_names()
+            else:
+                return tuple(key.split(CPK_SEP))
+
+        def separate_value(keys, value):
+            if isinstance(value, str):
+                return tuple(value.split(CPK_SEP))
+            elif isinstance(value, tuple):
+                return value
+            elif isinstance(value, list):
+                return tuple(value)
+            elif isinstance(value, dict):
+                new_vals = tuple(value.get(key) for key in keys)
+                return new_vals
+            else:
+                return (value,)
+
+        def transform_q(obj):
+            def make_q(keys, vals):
+                q = Q()
+                for key, val in zip(keys, vals):
+                    q.children.append((key, val))
+                return q
+
+            assert isinstance(obj, (Q, tuple))
+            if isinstance(obj, Q):
+                # When obj is Q, transform children.
+                new_q = copy.copy(obj)
+                new_q.children = []
+                for child in obj.children:
+                    new_q.children.append(transform_q(child))
+                return new_q
+            else:
+                # When obj is tuple,
+                #  obj[0] is lhs(lookup expression)
+                #       pk and multi column with lookup 'in' is nothing to do in this, it will change in 'names_to_path'. 
+                #  obj[1] is rhs(values)
+                #       valeus are separated in this method.
+                names = obj[0].split(LOOKUP_SEP)
+                if ('pk' in names and self.model.has_compositepk) or CPK_SEP in obj[0]:
+                    # When composite-pk or multi-column
+                    if len(names) == 1:
+                        # change one Q to multi Q
+                        keys = separate_key(self, obj[0])
+                        vals = separate_value(keys, obj[1])
+                        if len(keys) == len(vals):
+                            return make_q(keys, vals)
+                        else:
+                            raise ProgrammingError("Parameter unmatch : key={} val={}".format(keys, vals))
+                    else:
+                        # check the last name
+                        last = names[-1]
+                        if last == 'in':
+                            if len(names) == 2:
+                                # for 'pk__in' or 'multi-column__in'
+                                keys = separate_key(self, names[-2])
+                                new_vals = [separate_value(keys, val) for val in obj[1]]
+                                return (obj[0], new_vals)
+                            elif CPK_SEP in names[-2]:
+                                # multi-column is not supported.
+                                raise NotSupportedError("Not supported multi-column with'in' on relation model : {}".format(obj[0]))
+                        elif last == 'pk' or CPK_SEP in last:
+                            # change one Q to multi Q
+                            #  example: ('relmodel__id1,id2', (valule1,value2))
+                            #             |
+                            #             V
+                            #           ('relmodel__id1', valule1)
+                            #           ('relmodel__id2', valule2)
+                            before_path = LOOKUP_SEP.join(names[0:-1])
+                            cols = separate_key(self, last)
+                            keys = [before_path +  LOOKUP_SEP + col for col in cols]
+                            vals = separate_value(cols, obj[1])
+                            return make_q(keys, vals)
+                        else:
+                            # another lookup is not supported.
+                            raise NotSupportedError("Not supported multi-column with '{}' : {}".format(last,obj[0]))
+                return obj
+
+        new_q = transform_q(q_object)
+        super().add_q(new_q)
+
+
+class CPkQuery(CPkQueryMixin, Query):
+    pass
+
+
+class CPkDeleteQuery(CPkQueryMixin, DeleteQuery):
+    pass
+
+
+class CPkUpdateQuery(CPkQueryMixin, UpdateQuery):
+    pass
+
+
+class CPkQuerySet(QuerySet):
+    ###########################
+    # override
+    ###########################
+
+    def __init__(self, model=None, query=None, using=None, hints=None):
+        if not query:
+            query = CPkQuery(model)
+        super().__init__(model, query, using, hints)
+
+    def bulk_update(self, objs, fields, batch_size=None):
+        """
+        Update the given fields in each of the given objects in the database.
+        """
+        if batch_size is not None and batch_size < 0:
+            raise ValueError('Batch size must be a positive integer.')
+        if not fields:
+            raise ValueError('Field names must be given to bulk_update().')
+        objs = tuple(objs)
+        if any(obj.pk is None for obj in objs):
+            raise ValueError('All bulk_update() objects must have a primary key set.')
+        fields = [self.model._meta.get_field(name) for name in fields]
+        if any(not f.concrete or f.many_to_many for f in fields):
+            raise ValueError('bulk_update() can only be used with concrete fields.')
+        if any(f.primary_key for f in fields):
+            raise ValueError('bulk_update() cannot be used with primary key fields.')
+        if not objs:
+            return
+        # PK is used twice in the resulting update query, once in the filter
+        # and once in the WHEN. Each field will also have one CAST.
+        max_batch_size = connections[self.db].ops.bulk_batch_size(['pk', 'pk'] + fields, objs)
+        batch_size = min(batch_size, max_batch_size) if batch_size else max_batch_size
+        requires_casting = connections[self.db].features.requires_casted_case_in_updates
+        batches = (objs[i:i + batch_size] for i in range(0, len(objs), batch_size))
+        updates = []
+        for batch_objs in batches:
+            update_kwargs = {}
+            for field in fields:
+                when_statements = []
+                for obj in batch_objs:
+                    attr = getattr(obj, field.attname)
+                    if not isinstance(attr, Expression):
+                        attr = Value(attr, output_field=field)
+                    # CHANGE S
+                    #when_statements.append(When(pk=obj.pk, then=attr))
+                    lookups = obj.get_pk_lookups()
+                    when_statements.append(When(**lookups, then=attr))
+                    # CHANGE E
+                case_statement = Case(*when_statements, output_field=field)
+                if requires_casting:
+                    case_statement = Cast(case_statement, output_field=field)
+                update_kwargs[field.attname] = case_statement
+            updates.append(([obj.pk for obj in batch_objs], update_kwargs))
+        with transaction.atomic(using=self.db, savepoint=False):
+            for pks, update_kwargs in updates:
+                self.filter(pk__in=pks).update(**update_kwargs)
+    bulk_update.alters_data = True
```

