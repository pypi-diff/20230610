# Comparing `tmp/dbc-editor-0.4.0.tar.gz` & `tmp/dbc_editor-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbc-editor-0.4.0.tar", last modified: Sat Feb 18 10:17:38 2023, max compression
+gzip compressed data, was "dbc_editor-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dbc-editor-0.4.0.tar` & `dbc_editor-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      297 2022-11-28 07:33:17.189933 dbc-editor-0.4.0/.gitignore
--rw-r--r--   0        0        0      657 2022-11-03 16:33:53.710006 dbc-editor-0.4.0/LICENSE
--rw-r--r--   0        0        0     2156 2023-02-18 10:17:31.154650 dbc-editor-0.4.0/README.md
--rw-r--r--   0        0        0      699 2022-11-28 08:25:44.409977 dbc-editor-0.4.0/pyproject.toml
--rwxr-xr-x   0        0        0     9574 2022-11-28 07:25:34.774028 dbc-editor-0.4.0/release.sh
--rw-r--r--   0        0        0        5 2022-11-03 16:33:53.710006 dbc-editor-0.4.0/requirements-release.txt
--rw-r--r--   0        0        0       37 2022-11-28 07:40:01.146207 dbc-editor-0.4.0/requirements-test.txt
--rw-r--r--   0        0        0       23 2022-11-17 08:23:10.179477 dbc-editor-0.4.0/requirements.txt
--rw-r--r--   0        0        0       57 2023-02-07 12:45:15.178161 dbc-editor-0.4.0/src/dbc_editor/__init__.py
--rw-r--r--   0        0        0       77 2023-02-07 12:45:15.178161 dbc-editor-0.4.0/src/dbc_editor/__main__.py
--rw-r--r--   0        0        0     3605 2023-02-07 12:45:15.178161 dbc-editor-0.4.0/src/dbc_editor/config.py
--rwxr-xr-x   0        0        0    33315 2023-02-18 10:17:31.154650 dbc-editor-0.4.0/src/dbc_editor/main.py
--rw-r--r--   0        0        0     3406 2023-02-07 12:45:15.178161 dbc-editor-0.4.0/src/dbc_editor/model_input_history.py
--rwxr-xr-x   0        0        0      144 2023-02-07 12:45:15.178161 dbc-editor-0.4.0/src/dbc_editor/runmodule.sh
--rw-r--r--   0        0        0     1549 2023-02-07 12:45:15.178161 dbc-editor-0.4.0/src/dbc_editor/urwid_edit_with_history.py
--rw-r--r--   0        0        0      482 2022-11-28 07:39:26.276532 dbc-editor-0.4.0/tox.ini
--rw-r--r--   0        0        0     2816 1970-01-01 00:00:00.000000 dbc-editor-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      297 2022-11-28 07:33:17.189933 dbc_editor-0.5.0/.gitignore
+-rw-r--r--   0        0        0      657 2022-11-03 16:33:53.710006 dbc_editor-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2141 2023-06-10 08:01:38.883781 dbc_editor-0.5.0/README.md
+-rw-r--r--   0        0        0      699 2022-11-28 08:25:44.409977 dbc_editor-0.5.0/pyproject.toml
+-rwxr-xr-x   0        0        0     9574 2022-11-28 07:25:34.774028 dbc_editor-0.5.0/release.sh
+-rw-r--r--   0        0        0        5 2022-11-03 16:33:53.710006 dbc_editor-0.5.0/requirements-release.txt
+-rw-r--r--   0        0        0       37 2022-11-28 07:40:01.146207 dbc_editor-0.5.0/requirements-test.txt
+-rw-r--r--   0        0        0       23 2022-11-17 08:23:10.179477 dbc_editor-0.5.0/requirements.txt
+-rw-r--r--   0        0        0       57 2023-02-07 12:45:15.178161 dbc_editor-0.5.0/src/dbc_editor/__init__.py
+-rw-r--r--   0        0        0       77 2023-02-07 12:45:15.178161 dbc_editor-0.5.0/src/dbc_editor/__main__.py
+-rw-r--r--   0        0        0     3605 2023-02-07 12:45:15.178161 dbc_editor-0.5.0/src/dbc_editor/config.py
+-rwxr-xr-x   0        0        0    39706 2023-06-10 08:01:38.883781 dbc_editor-0.5.0/src/dbc_editor/main.py
+-rw-r--r--   0        0        0     3406 2023-02-07 12:45:15.178161 dbc_editor-0.5.0/src/dbc_editor/model_input_history.py
+-rwxr-xr-x   0        0        0      144 2023-02-07 12:45:15.178161 dbc_editor-0.5.0/src/dbc_editor/runmodule.sh
+-rw-r--r--   0        0        0     1549 2023-02-07 12:45:15.178161 dbc_editor-0.5.0/src/dbc_editor/urwid_edit_with_history.py
+-rw-r--r--   0        0        0      482 2022-11-28 07:39:26.276532 dbc_editor-0.5.0/tox.ini
+-rw-r--r--   0        0        0     2801 1970-01-01 00:00:00.000000 dbc_editor-0.5.0/PKG-INFO
```

### Comparing `dbc-editor-0.4.0/LICENSE` & `dbc_editor-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbc-editor-0.4.0/README.md` & `dbc_editor-0.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -50,11 +50,10 @@
 
 Missing message attributes:
 - senders
 - send_type
 - cycle_time
 
 Missing signal attributes:
-- multiplexing
 - initial
 - minimum
 - maximum
```

### Comparing `dbc-editor-0.4.0/pyproject.toml` & `dbc_editor-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbc-editor-0.4.0/release.sh` & `dbc_editor-0.5.0/release.sh`

 * *Files identical despite different names*

### Comparing `dbc-editor-0.4.0/src/dbc_editor/config.py` & `dbc_editor-0.5.0/src/dbc_editor/config.py`

 * *Files identical despite different names*

### Comparing `dbc-editor-0.4.0/src/dbc_editor/main.py` & `dbc_editor-0.5.0/src/dbc_editor/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!./runmodule.sh
 
 '''
 An editor for CAN bus database files like dbc or sym, based on cantools and urwid
 '''
 
-__version__ = '0.4.0'
+__version__ = '0.5.0'
 
 
 import os
 import sys
 import argparse
 import tempfile
 import logging
@@ -189,14 +189,37 @@
 			return self.default_value
 		return int(self.get_edit_text())
 
 	def set_value(self, value: int) -> None:
 		self.set_edit_text(format(value, self.fmt))
 		self.set_edit_pos(len(self.get_edit_text()))
 
+class UintListEdit(EditBaseClass):
+
+	fmt = '%s'
+
+	# override method of super class
+	def valid_char(self, ch: str) -> bool:
+		return ch.lower() in '0123456789xABCDEFabcdef, '
+
+	def check(self) -> bool:
+		try:
+			self.value()
+			return True
+		except ValueError:
+			return False
+
+	def value(self) -> 'list[int]':
+		return [int(i, base=0) for i in self.get_edit_text().split(',')]
+
+	def set_value(self, value: 'list[int]') -> None:
+		self.set_edit_text(', '.join(self.fmt % i for i in value))
+		self.set_edit_pos(len(self.get_edit_text()))
+
+
 class FloatEdit(EditBaseClass):
 
 	def __init__(self, caption: str, *, default_value: 'float|None' = None, fmt: str = '') -> None:
 		super().__init__(caption=caption)
 		self.default_value = default_value
 		self.fmt = fmt
 
@@ -232,15 +255,15 @@
 
 	def pack(self, size=None, focus=False):
 		text = ' '*self.reserve_columns + self.get_label()
 		return urwid.Text(text).pack(size=size, focus=focus)
 
 class ChoiceEdit(urwid.Columns):
 
-	def __init__(self, caption: str, *, choices: 'list[str], dict[str, T]') -> None:
+	def __init__(self, caption: str, *, choices: 'list[str]|dict[str, T]') -> None:
 		self.caption = caption
 		self.choices: 'dict[str, T]' = choices if isinstance(choices, dict) else {v:v for v in choices}
 		buttons_group = []
 		self.caption = urwid.Text(caption)
 		self.radio_buttons = {key: PackableRadioButton(buttons_group, key) for key in list(choices)}
 		widgets = [self.caption] + list(self.radio_buttons.values())
 		widget_list = [('pack', w) for w in widgets]
@@ -508,34 +531,38 @@
 	def cmd_remove(self):
 		self.db.messages.remove(self.get_selected_message())
 		self.update()
 		self.app.notify_has_changed()
 
 class MessageLineWidget(LineWidget):
 
-	fmt_line = Config('message-list.fmt', '{msg.frame_id:>6x} {msg.name}  (DLC: {msg.length}, bytes used: {bytes_used})')
+	fmt_line = Config('message-list.fmt', '{msg.frame_id:>0{frame_id_width}x} {msg.name}  (DLC: {msg.length}, bytes used: {bytes_used})')
 
 	def __init__(self, msg):
 		bytes_used = sum(sig.length for sig in msg.signals) / 8.0
 		if bytes_used.is_integer():
 			bytes_used = int(bytes_used)
-		super().__init__(self.fmt_line.format(msg=msg, bytes_used=bytes_used))
+		ln = self.fmt_line.format(msg=msg, bytes_used=bytes_used,
+			frame_format = "ext" if msg.is_extended_frame else "std",
+			frame_id_width = 8 if msg.is_extended_frame else 3,
+		)
+		super().__init__(ln)
 		self.msg = msg
 
 
 class MessageEdit(MyWindow):
 
 	title_edit = 'edit message {msg.frame_id:03x} {msg.name}'
 	title_new = 'create new message'
 
 	def __init__(self, db, msg=None, **kw):
 		self.db = db
 		self.msg = msg
-		self.edit_frame_id = HexEdit("Frame ID: ")
-		self.edit_is_extended_frame = ChoiceEdit("Is extended: ", choices=dict(true=True, false=False))
+		self.edit_frame_id = HexEdit("Frame ID (hex): ")
+		self.edit_is_extended_frame = ChoiceEdit("", choices={"Extended Frame": True, "Standard Frame": False})
 		self.edit_name = TextEdit("Message Name: ")
 		self.edit_comment = OptionalTextEdit("Comment: ")
 		self.edit_length = UintEdit("Data length (in bytes): ", default_value=0)
 
 		if msg:
 			title = self.title_edit.format(msg=msg)
 			for key in ('frame_id', 'is_extended_frame', 'name', 'comment', 'length'):
@@ -685,14 +712,15 @@
 	def __init__(self, msg, **kw):
 		self.msg = msg
 
 		title = self.title.format(msg=msg)
 		shortcuts = [
 			('up/down', 'select signal'),
 			('+', 'new signal'),
+			('=', 'copy signal'),
 			('-', 'delete signal'),
 			('i', 'edit signal'),
 			('q', 'quit')
 		]
 		body = [MyAttrMap(SignalLineWidget(sig)) for sig in sorted(self.msg.signals, key=lambda sig: sig.start)]
 		body = MyListBox(body)
 
@@ -701,26 +729,36 @@
 		self.set_help_line(shortcuts)
 
 	def update(self):
 		body = [MyAttrMap(SignalLineWidget(sig)) for sig in sorted(self.msg.signals, key=lambda sig: sig.start)]
 		body = MyListBox(body)
 		self.set_body(body)
 
+	def select_signal(self, signal) -> None:
+		for i, widget in enumerate(self.body.body):
+			widget = widget.base_widget
+			if widget.signal == signal:
+				self.body.body.set_focus(i)
+				return
+
 	def get_selected_signal(self):
 		return self.body.focus.base_widget.signal
 
 	def cmd_open(self):
 		return SignalEdit(self.msg, self.get_selected_signal(), prev_window=self)
 
 	def cmd_edit(self):
 		return SignalEdit(self.msg, self.get_selected_signal(), prev_window=self)
 
 	def cmd_new(self):
 		return SignalEdit(self.msg, prev_window=self)
 
+	def cmd_copy(self):
+		return SignalEdit(self.msg, self.get_selected_signal(), copy=True, prev_window=self)
+
 	def cmd_remove(self):
 		self.msg.signals.remove(self.get_selected_signal())
 		self.update()
 		self.app.notify_has_changed()
 
 
 	def get_selected_message(self) -> cantools.database.Message:
@@ -766,33 +804,49 @@
 	BYTE_ORDER = {
 		'Little Endian / Intel' : 'little_endian',
 		'Big Endian / Motorola' : 'big_endian',
 	}
 
 	default_byte_order = Config('signal-edit.default-byte-order', 'little_endian', allowed_values=BYTE_ORDER.values())
 
-	def __init__(self, msg, sig=None, **kw):
+	def __init__(self, msg, sig=None, *, copy: bool = False, **kw):
 		self.msg = msg
 		self.sig = sig
+		self.copy = copy
 		self.edit_name = TextEdit("Signal Name: ")
 		self.edit_start = UintEdit("Start Bit: ")
 		self.edit_length = UintEdit("Length (number of bits): ")
 		self.edit_byte_order = ChoiceEdit("Byte Order: ", choices=self.BYTE_ORDER)
 		self.edit_type = ChoiceEdit("Type: ", choices=self.TYPES)
 		# Factor by which the raw value transmitted via the CAN bus must be multiplied in order to get the specified unit
 		self.edit_scale = FloatEdit("Scale: ", default_value=1)
 		# Summand by which the scaled value must be added in order to get the specified unit
 		self.edit_offset = FloatEdit("Offset: ", default_value=0)
 		self.edit_unit = OptionalTextEdit("Unit: ")
 		self.edit_comment = OptionalTextEdit("Comment: ")
 		self.text_value_range = urwid.Text("")
+		self.edit_is_multiplexer = ChoiceEdit("Is multiplexer: ", choices={'true': True, 'false': False})
+		self.edit_is_multiplexer.set_value(False)
+		self.edit_is_multiplexed = ChoiceEdit("Depends on the value of another signal", choices={'true': True, 'false': False})
+		self.edit_multiplexer_signal = ChoiceEdit("Multiplexer signal: ", choices=[s.name for s in msg.signals if s.is_multiplexer])
+		self.edit_multiplexer_ids = UintListEdit("Multiplexer IDs: ")
+		self.pile_multiplexed = urwid.Pile([self.edit_multiplexer_signal, self.edit_multiplexer_ids])
+		self.pile_not_multiplexed = urwid.Text("")
+		self.edit_is_multiplexed.set_value(False)
+		for s in msg.signals:
+			if s.is_multiplexer:
+				self.edit_multiplexer_signal.set_value(s.name)
+		self.placeholder_multiplexed = urwid.WidgetWrap(self.pile_not_multiplexed)
+		self.edit_is_multiplexed.register_on_change_listener(self.change_is_multipexed)
 
+		self.choices_input_mode_selector = ChoiceEdit('choice key', choices=('dec', 'hex'))
+		self.choices_input_mode_selector.register_on_change_listener(self.change_choices_input_mode)
 		self.choices_group: 'list[ChoiceLineEdit]' = []
 		ChoiceLineEdit(self.choices_group, self.update_pile_choices)
-		self.pile_choices = urwid.Pile(self.choices_group)
+		self.pile_choices = urwid.Pile([self.choices_input_mode_selector] + self.choices_group)
 		self.pile_number = urwid.Pile([
 			self.edit_scale,
 			self.edit_offset,
 			self.edit_unit,
 		])
 		self.placeholder = urwid.WidgetWrap(self.pile_number)
 		self.edit_type.register_on_change_listener(self.on_type_change)
@@ -810,14 +864,20 @@
 				self.edit_type.set_value(self.TYPE_CHOICES)
 			elif sig.is_float:
 				self.edit_type.set_value(self.TYPE_FLOAT)
 			elif sig.is_signed:
 				self.edit_type.set_value(self.TYPE_SIGNED_INT)
 			else:
 				self.edit_type.set_value(self.TYPE_UNSIGNED_INT)
+			if sig.is_multiplexer:
+				self.edit_is_multiplexer.set_value(True)
+			if sig.multiplexer_signal:
+				self.edit_is_multiplexed.set_value(True)
+				self.edit_multiplexer_signal.set_value(sig.multiplexer_signal)
+				self.edit_multiplexer_ids.set_value(sig.multiplexer_ids)
 		else:
 			self.edit_byte_order.set_value(self.default_byte_order)
 			#TODO: does this work for big endian, too?
 			if self.msg.signals:
 				last_signal = self.msg.signals[-1]
 				self.edit_start.set_value(last_signal.start + last_signal.length)
 			else:
@@ -829,22 +889,38 @@
 			self.edit_name,
 			self.edit_length,
 			self.edit_type,
 			self.placeholder,
 			self.edit_comment,
 			self.edit_byte_order,
 			self.text_value_range,
+			self.edit_is_multiplexer,
+			self.edit_is_multiplexed,
+			self.placeholder_multiplexed,
 		])
 		filler = urwid.Filler(pile)
 
 		super().__init__(filler, **kw)
 		self.set_title(title)
 		self.init_value_range()
 		pile.set_focus(1)
 
+	def change_choices_input_mode(self, widget: ChoiceEdit, value: str) -> None:
+		if value == 'hex':
+			for w in self.choices_group:
+				w.set_input_mode_to_hex()
+		elif value == 'dec':
+			for w in self.choices_group:
+				w.set_input_mode_to_dec()
+		else:
+			assert False, f'invalid value {value} should be hex or dec'
+
+	def change_is_multipexed(self, widget: ChoiceEdit, value: bool) -> None:
+		self.placeholder_multiplexed._w = self.pile_multiplexed if value else self.pile_not_multiplexed
+
 	def init_value_range(self) -> None:
 		dependencies = (
 			self.edit_length,
 			self.edit_type,
 			self.edit_scale,
 			self.edit_offset,
 			self.edit_unit,
@@ -892,15 +968,15 @@
 	def on_type_change(self, widget, value) -> None:
 		if value == self.TYPE_CHOICES:
 			self.placeholder._w = self.pile_choices
 		else:
 			self.placeholder._w = self.pile_number
 
 	def update_pile_choices(self) -> None:
-		self.pile_choices = urwid.Pile(self.choices_group, focus_item=self.pile_choices.get_focus())
+		self.pile_choices = urwid.Pile([self.choices_input_mode_selector] + self.choices_group, focus_item=self.pile_choices.get_focus())
 		self.placeholder._w = self.pile_choices
 
 
 	def get_input_data(self):
 		dtype = self.edit_type.value()
 		if dtype and dtype not in self.TYPES:
 			raise ValueError('invalid type %r, should be one of %s' % (dtype, self.TYPES))
@@ -913,36 +989,89 @@
 		out['is_float'] = dtype == self.TYPE_FLOAT
 		out['byte_order'] = self.edit_byte_order.value()
 		out['scale'] = self.edit_scale.value()
 		out['offset'] = self.edit_offset.value()
 		out['unit'] = self.edit_unit.value()
 		out['comment'] = self.edit_comment.value()
 		out['choices'] = {c.edit_value.value() : c.edit_name.value() for c in self.choices_group if c.edit_name.check()} if dtype == self.TYPE_CHOICES else None
+		out['is_multiplexer'] = self.edit_is_multiplexer.value()
+		if self.edit_is_multiplexed.value():
+			out['multiplexer_signal'] = self.edit_multiplexer_signal.value()
+			out['multiplexer_ids'] = self.edit_multiplexer_ids.value()
+		else:
+			out['multiplexer_signal'] = None
+			out['multiplexer_ids'] = None
 		return out
 
 	def check(self, *, silent: bool = False) -> bool:
 		if self.edit_type.value() == self.TYPE_CHOICES:
 			placeholder_edits = tuple(c.edit_value for c in self.choices_group if c.edit_name.check())
 		else:
 			placeholder_edits = tuple(widget for widget, options in self.pile_number.contents)
+		if self.edit_is_multiplexed.value():
+			placeholder_mux = (self.edit_multiplexer_signal, self.edit_multiplexer_ids)
+		else:
+			placeholder_mux = tuple()
 		for w in (
 			self.edit_name,
 			self.edit_start,
 			self.edit_length,
 			self.edit_type,
 			self.edit_byte_order,
 			self.edit_comment,
-		) + placeholder_edits:
+			self.edit_is_multiplexer,
+			self.edit_is_multiplexed,
+		) + placeholder_edits + placeholder_mux:
 			if not w.check():
 				if not silent:
 					self.show_error('Invalid input for %s' % w.caption.rstrip().rstrip(':'))
 				return False
 
+		if self.edit_is_multiplexer.value() == False:
+			multiplexed_signals = self.get_signals_depending_on_this_signal()
+			if multiplexed_signals:
+				if not silent:
+					self.show_error('This signal cannot be disabled as a multiplexer because the following signals depend on it: %s' % ', '.join(s.name for s in multiplexed_signals))
+				return False
+
+		if self.edit_is_multiplexed.value():
+			try:
+				multiplexer_signal = self.msg.get_signal_by_name(self.edit_multiplexer_signal.value())
+			except KeyError:
+				if not silent:
+					self.show_error('This message does not have a signal named %r' % self.edit_multiplexer_signal.value())
+				return False
+			if multiplexer_signal.name == self.edit_name.value():
+				if not silent:
+					self.show_error('This signal cannot be multiplexed by itself')
+				return False
+			if not multiplexer_signal.is_multiplexer:
+				if not silent:
+					self.show_error('%s is not multiplexer' % multiplexer_signal)
+				#return False
+
+			multiplexer_ids = self.edit_multiplexer_ids.value()
+			if not multiplexer_ids:
+				if not silent:
+					self.show_error('No multiplexer IDs specified which would activate this signal')
+				return False
+			id_too_big = 1 << multiplexer_signal.length
+			for i in multiplexer_ids:
+				if i >= id_too_big:
+					if not silent:
+						self.show_error(f'Multiplexer ID {i} is too big, {multiplexer_signal.name} is only {multiplexer_signal.length} bits long')
+					return False
+
 		return True
 
+	def get_signals_depending_on_this_signal(self) -> 'list[cantools.db.Signal]':
+		if not self.sig:
+			return []
+		return [s for s in self.msg.signals if s.multiplexer_signal == self.sig.name]
+
 	def has_changed(self):
 		if not self.sig:
 			return True
 
 		if not self.check(silent=True):
 			return True
 
@@ -968,22 +1097,32 @@
 
 		return super().cmd_back()
 
 	def reply_save(self):
 		if not self.check():
 			return
 
-		if self.sig:
+		if self.sig and not self.copy:
 			for attr, value in self.get_input_data().items():
+				if attr == 'name' and self.sig.name != value:
+					for s in self.get_signals_depending_on_this_signal():
+						s.multiplexer_signal = value
 				setattr(self.sig, attr, value)
 		else:
 			newsig = cantools.database.Signal(**self.get_input_data())
-			self.msg.signals.append(newsig)
+			if self.sig:
+				i = self.msg.signals.index(self.sig) + 1
+			else:
+				i = len(self.msg.signals)
+			self.msg.signals.insert(i, newsig)
+			self.sig = newsig
+			self.copy = False
 
 		self.prev_window.update()
+		self.prev_window.select_signal(self.sig)
 		self.app.notify_has_changed()
 		return self.cmd_cancel()
 
 	def reply_dont_save(self):
 		return self.cmd_cancel()
 
 	def reply_cancel(self):
@@ -993,33 +1132,31 @@
 	def get_selected_message(self) -> cantools.database.Message:
 		return self.msg
 
 
 
 class ChoiceLineEdit(urwid.Columns):
 
-	value_width = 3
+	min_value_width = 3
 
 	# ------- init -------
 
-	def __init__(self, group: 'list[ChoiceLineEdit]', update_pile: 'Callable[[], None]', *, before: 'ChoiceLineEdit|None' = None) -> None:
+	def __init__(self, group: 'list[ChoiceLineEdit]', update_pile: 'Callable[[], None]', *, before: 'ChoiceLineEdit|None' = None, value_edit_type: 'type[UintEdit|HexEdit]' = UintEdit) -> None:
 		self.group = group
 		self.update_pile = update_pile
-		self.edit_value = UintEdit('')
+		self.edit_value: 'UintEdit|HexEdit' = value_edit_type('')
 		self.edit_name = TextEdit('')
 
 		if before is None:
 			group.append(self)
 		else:
 			group.insert(group.index(before), self)
 		self.init_value()
-		super().__init__([
-			(self.value_width, self.edit_value),
-			self.edit_name,
-		], dividechars=1)
+		super().__init__([], dividechars=1)
+		self._update_widgets()
 		self.edit_name.register_on_change_listener(lambda w, v: self.add_after_if_last())
 
 	def init_value(self) -> None:
 		prev = self.get_prev_value()
 		self.edit_value.set_value(0 if prev is None else prev+1)
 
 	def get_prev_value(self) -> 'int|None':
@@ -1030,37 +1167,59 @@
 				return prev_widget.edit_value.value()
 			i -= 1
 		return None
 
 	def set_value(self, value: int, name: str) -> None:
 		self.edit_value.set_value(value)
 		self.edit_name.set_value(name)
+		self._update_widgets()
+
+	def set_input_mode_to_hex(self) -> None:
+		val = self.edit_value.value()
+		self.edit_value = HexEdit('')
+		self.edit_value.set_value(val)
+		self._update_widgets()
+
+	def set_input_mode_to_dec(self) -> None:
+		val = self.edit_value.value()
+		self.edit_value = UintEdit('')
+		self.edit_value.set_value(val)
+		self._update_widgets()
+
+	def _update_widgets(self) -> None:
+		needed_with = len(self.edit_value.get_text()[0])
+		value_width = max(self.min_value_width, needed_with)
+		value_width += 1
+		self.contents = [
+			(self.edit_value, self.options('given', value_width)),
+			(self.edit_name, self.options('weight', 1)),
+		]
 
 	# ------- events -------
 
 	def add_after_if_last(self) -> None:
 		i = self.group.index(self)
 		if i < len(self.group) - 1:
 			return
 
-		ChoiceLineEdit(self.group, self.update_pile)
+		ChoiceLineEdit(self.group, self.update_pile, value_edit_type=type(self.edit_value))
 		self.update_pile()
 
 	#TODO: this is not called. Does the UintEdit gobble the event?
 	def cmd_new(self) -> None:
 		self.add_before()
 
 	#TODO: this is not called. Does the UintEdit gobble the event?
 	def cmd_remove(self) -> None:
 		self.group.remove(self)
 		#TODO: decrement numbers of following
 		self.update_pile()
 
 	def add_before(self) -> None:
-		ChoiceLineEdit(self.group, self.update_pile, before=self)
+		ChoiceLineEdit(self.group, self.update_pile, before=self, value_edit_type=type(self.edit_value))
 		#TODO: change duplicate numbers
 		self.update_pile()
 
 
 # ------- main classes -------
 
 class UserInputError(Exception):
@@ -1079,14 +1238,15 @@
 	command_map = urwid.command_map
 	command_map['w'] = 'write'
 	command_map['q'] = 'quit'
 	command_map['e'] = 'edit'
 	command_map['i'] = 'edit'
 	command_map['esc'] = 'cancel'
 	command_map['+'] = 'new'
+	command_map['='] = 'copy'
 	command_map['-'] = 'remove'
 	command_map['/'] = 'search'
 	command_map['?'] = 'search_reverse'
 	command_map['v'] = 'message_layout'
 
 	fallback_commands = {
 		'activate' : 'open',
```

### Comparing `dbc-editor-0.4.0/src/dbc_editor/model_input_history.py` & `dbc_editor-0.5.0/src/dbc_editor/model_input_history.py`

 * *Files identical despite different names*

### Comparing `dbc-editor-0.4.0/src/dbc_editor/urwid_edit_with_history.py` & `dbc_editor-0.5.0/src/dbc_editor/urwid_edit_with_history.py`

 * *Files identical despite different names*

### Comparing `dbc-editor-0.4.0/PKG-INFO` & `dbc_editor-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbc-editor
-Version: 0.4.0
+Version: 0.5.0
 Summary: An editor for CAN bus database files like dbc or sym, based on cantools and urwid
 Author-email: erzo <erzo@posteo.de>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
@@ -67,12 +67,11 @@
 
 Missing message attributes:
 - senders
 - send_type
 - cycle_time
 
 Missing signal attributes:
-- multiplexing
 - initial
 - minimum
 - maximum
```

