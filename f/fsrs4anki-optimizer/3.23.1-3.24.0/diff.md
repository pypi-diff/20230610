# Comparing `tmp/fsrs4anki_optimizer-3.23.1.tar.gz` & `tmp/fsrs4anki_optimizer-3.24.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-3.23.1.tar", last modified: Thu Jun  8 20:49:25 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-3.24.0.tar", last modified: Sat Jun 10 13:45:30 2023, max compression
```

## Comparing `fsrs4anki_optimizer-3.23.1.tar` & `fsrs4anki_optimizer-3.24.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:49:25.701580 fsrs4anki_optimizer-3.23.1/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-08 20:49:25.701580 fsrs4anki_optimizer-3.23.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:49:25.701580 fsrs4anki_optimizer-3.23.1/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-08 20:49:06.000000 fsrs4anki_optimizer-3.23.1/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-08 20:49:06.000000 fsrs4anki_optimizer-3.23.1/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43276 2023-06-08 20:49:06.000000 fsrs4anki_optimizer-3.23.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:49:25.701580 fsrs4anki_optimizer-3.23.1/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-08 20:49:25.000000 fsrs4anki_optimizer-3.23.1/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-08 20:49:25.000000 fsrs4anki_optimizer-3.23.1/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:49:25.000000 fsrs4anki_optimizer-3.23.1/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-08 20:49:25.000000 fsrs4anki_optimizer-3.23.1/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 20:49:25.000000 fsrs4anki_optimizer-3.23.1/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-08 20:49:06.000000 fsrs4anki_optimizer-3.23.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 20:49:25.701580 fsrs4anki_optimizer-3.23.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-08 20:49:06.000000 fsrs4anki_optimizer-3.23.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:45:30.227906 fsrs4anki_optimizer-3.24.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-10 13:45:30.227906 fsrs4anki_optimizer-3.24.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:45:30.223906 fsrs4anki_optimizer-3.24.0/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-10 13:45:18.000000 fsrs4anki_optimizer-3.24.0/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-10 13:45:18.000000 fsrs4anki_optimizer-3.24.0/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43138 2023-06-10 13:45:18.000000 fsrs4anki_optimizer-3.24.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 13:45:30.227906 fsrs4anki_optimizer-3.24.0/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-10 13:45:30.000000 fsrs4anki_optimizer-3.24.0/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-10 13:45:30.000000 fsrs4anki_optimizer-3.24.0/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 13:45:30.000000 fsrs4anki_optimizer-3.24.0/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-10 13:45:30.000000 fsrs4anki_optimizer-3.24.0/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-10 13:45:30.000000 fsrs4anki_optimizer-3.24.0/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-10 13:45:18.000000 fsrs4anki_optimizer-3.24.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 13:45:30.227906 fsrs4anki_optimizer-3.24.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-10 13:45:18.000000 fsrs4anki_optimizer-3.24.0/setup.py
```

### Comparing `fsrs4anki_optimizer-3.23.1/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-3.24.0/fsrs4anki_optimizer/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,25 +71,29 @@
     with open(config_save, "w+") as f: # Save the settings to load next time the program is run
         json.dump(remembered_fallbacks, f)
 
     show_graphs = graphs_input != "n"
 
     optimizer = fsrs4anki_optimizer.Optimizer()
     optimizer.anki_extract(args.filename)
-    optimizer.create_time_series(
+    analysis = optimizer.create_time_series(
         remembered_fallbacks["timezone"],
         remembered_fallbacks["revlog_start_date"],
         remembered_fallbacks["next_day"]
     )
+    print(analysis)
 
     optimizer.define_model()
     optimizer.train()
 
     optimizer.predict_memory_states()
-    optimizer.find_optimal_retention(show_graphs)
+    figures = optimizer.find_optimal_retention()
+    if show_graphs:
+        for f in figures:
+            f.show()
 
     optimizer.preview(optimizer.optimal_retention)
 
     profile = \
 f"""{{
     // Generated, Optimized anki deck settings
     // Need to add <div id=deck deck_name="{{{{Deck}}}}"></div> to your card's front template's first line.
@@ -105,10 +109,13 @@
     print("Paste this into your scheduling code")
     print(profile)
     
     if args.out:
         with open(args.out, "a+") as f:
             f.write(profile)
 
+    optimizer.evaluate()
     if show_graphs:
-        optimizer.evaluate()
-        optimizer.calibration_graph()
+        for f in optimizer.calibration_graph():
+            f.show()
+        for f in optimizer.compare_with_sm2():
+            f.show()
```

### Comparing `fsrs4anki_optimizer-3.23.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-3.24.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,27 +13,18 @@
 import torch
 from torch import nn
 from torch.utils.data import Dataset, DataLoader, Sampler
 from torch.nn.utils.rnn import pad_sequence, pack_padded_sequence, pad_packed_sequence
 from sklearn.model_selection import StratifiedGroupKFold
 from sklearn.metrics import mean_squared_error, r2_score
 from itertools import accumulate
+from tqdm.auto import tqdm
 import warnings
 warnings.filterwarnings("ignore", category=UserWarning)
 
-def is_interactive(): # https://stackoverflow.com/questions/15411967/how-can-i-check-if-code-is-executed-in-the-ipython-notebook
-    import __main__ as main
-    return not hasattr(main, '__file__')
-
-if is_interactive():
-    from tqdm import notebook
-else:
-    # Export cli module pretending to be notebook if not in notebook
-    from tqdm import cli as notebook 
-
 class FSRS(nn.Module):
     def __init__(self, w):
         super(FSRS, self).__init__()
         self.w = nn.Parameter(torch.tensor(w, dtype=torch.float32))
 
     def stability_after_success(self, state, new_d, r):
         new_s = state[:,0] * (1 + torch.exp(self.w[6]) *
@@ -204,15 +195,15 @@
         # pretrain
         best_loss = np.inf
         weighted_loss, w = self.eval()
         if weighted_loss < best_loss:
             best_loss = weighted_loss
             best_w = w
 
-        pbar = notebook.tqdm(desc="pre-train", colour="red", total=len(self.pre_train_data_loader) * self.n_epoch)
+        pbar = tqdm(desc="pre-train", colour="red", total=len(self.pre_train_data_loader) * self.n_epoch, )
         for k in range(self.n_epoch):
             for i, batch in enumerate(self.pre_train_data_loader):
                 self.model.train()
                 self.optimizer.zero_grad()
                 sequences, delta_ts, labels, seq_lens = batch
                 real_batch_size = seq_lens.shape[0]
                 outputs, _ = self.model(sequences)
@@ -225,15 +216,15 @@
                 pbar.update(n=real_batch_size)
 
         pbar.close()
         for name, param in self.model.named_parameters():
             print(f"{name}: {list(map(lambda x: round(float(x), 4),param))}")
 
         epoch_len = len(self.next_train_data_loader)
-        pbar = notebook.tqdm(desc="train", colour="red", total=epoch_len*self.n_epoch)
+        pbar = tqdm(desc="train", colour="red", total=epoch_len*self.n_epoch)
         print_len = max(self.batch_nums*self.n_epoch // 10, 1)
         for k in range(self.n_epoch):
             weighted_loss, w = self.eval()
             if weighted_loss < best_loss:
                 best_loss = weighted_loss
                 best_w = w
 
@@ -251,17 +242,17 @@
                     param.grad[:2] = torch.zeros(2)
                 self.optimizer.step()
                 self.scheduler.step()
                 self.model.apply(self.clipper)
                 pbar.update(real_batch_size)
 
                 if (k * self.batch_nums + i + 1) % print_len == 0:
-                    print(f"iteration: {k * epoch_len + (i + 1) * self.batch_size}")
+                    tqdm.write(f"iteration: {k * epoch_len + (i + 1) * self.batch_size}")
                     for name, param in self.model.named_parameters():
-                        print(f"{name}: {list(map(lambda x: round(float(x), 4),param))}")
+                        tqdm.write(f"{name}: {list(map(lambda x: round(float(x), 4),param))}")
         pbar.close()
 
         weighted_loss, w = self.eval()
         if weighted_loss < best_loss:
             best_loss = weighted_loss
             best_w = w
 
@@ -273,38 +264,40 @@
             sequences, delta_ts, labels, seq_lens = self.train_set.x_train, self.train_set.t_train, self.train_set.y_train, self.train_set.seq_len
             real_batch_size = seq_lens.shape[0]
             outputs, _ = self.model(sequences.transpose(0, 1))
             stabilities = outputs[seq_lens-1, torch.arange(real_batch_size), 0]
             retentions = torch.exp(np.log(0.9) * delta_ts / stabilities)
             tran_loss = self.loss_fn(retentions, labels)/len(self.train_set)
             self.avg_train_losses.append(tran_loss)
-            print(f"Loss in trainset: {tran_loss:.4f}")
+            tqdm.write(f"Loss in trainset: {tran_loss:.4f}")
 
             sequences, delta_ts, labels, seq_lens = self.test_set.x_train, self.test_set.t_train, self.test_set.y_train, self.test_set.seq_len
             real_batch_size = seq_lens.shape[0]
             outputs, _ = self.model(sequences.transpose(0, 1))
             stabilities = outputs[seq_lens-1, torch.arange(real_batch_size), 0]
             retentions = torch.exp(np.log(0.9) * delta_ts / stabilities)
             test_loss = self.loss_fn(retentions, labels)/len(self.test_set)
             self.avg_eval_losses.append(test_loss)
-            print(f"Loss in testset: {test_loss:.4f}")
+            tqdm.write(f"Loss in testset: {test_loss:.4f}")
 
             w = list(map(lambda x: round(float(x), 4), dict(self.model.named_parameters())['w'].data))
 
             weighted_loss = (tran_loss * len(self.train_set) + test_loss * len(self.test_set)) / (len(self.train_set) + len(self.test_set))
 
             return weighted_loss, w
 
     def plot(self):
-        plt.plot(self.avg_train_losses, label='train')
-        plt.plot(self.avg_eval_losses, label='test')
-        plt.xlabel('epoch')
-        plt.ylabel('loss')
-        plt.legend()
-        plt.show()
+        fig = plt.figure()
+        ax = fig.gca()
+        ax.plot(self.avg_train_losses, label='train')
+        ax.plot(self.avg_eval_losses, label='test')
+        ax.set_xlabel('epoch')
+        ax.set_ylabel('loss')
+        ax.legend()
+        return fig
 
 class Collection:
     def __init__(self, w):
         self.model = FSRS(w)
         self.model.eval()
 
     def predict(self, t_history, r_history):
@@ -318,16 +311,15 @@
         outputs, _ = self.model(fast_dataset.x_train.transpose(0, 1))
         stabilities, difficulties = outputs[fast_dataset.seq_len-1, torch.arange(len(fast_dataset))].transpose(0, 1)
         return stabilities.tolist(), difficulties.tolist()
 
 """Used to store all the results from FSRS related functions"""
 class Optimizer:
     def __init__(self) -> None:
-        notebook.tqdm.pandas()
-        pass
+        tqdm.pandas()
 
     @staticmethod
     def anki_extract(filename: str):
         """Step 1"""
         # Extract the collection file or deck file to get the .anki21 database.
         with zipfile.ZipFile(f'{filename}', 'r') as zip_ref:
             zip_ref.extractall('./')
@@ -428,26 +420,27 @@
         df = df.groupby(by=['r_history'], group_keys=False).progress_apply(cal_stability)
         print("Stability calculated.")
         df.reset_index(drop = True, inplace = True)
         df.drop_duplicates(inplace=True)
         df.sort_values(by=['r_history'], inplace=True, ignore_index=True)
 
         if df.shape[0] > 0:
-            for idx in notebook.tqdm(df.index):
+            for idx in tqdm(df.index):
                 item = df.loc[idx]
                 index = df[(df['i'] == item['i'] + 1) & (df['r_history'].str.startswith(item['r_history']))].index
                 df.loc[index, 'last_stability'] = item['stability']
             df['factor'] = round(df['stability'] / df['last_stability'], 2)
             df = df[(df['i'] >= 2) & (df['group_cnt'] >= 100)].copy()
             df['last_recall'] = df['r_history'].map(lambda x: x[-1])
             df = df[df.groupby(['i', 'r_history'], group_keys=False)['group_cnt'].transform(max) == df['group_cnt']]
             df.to_csv('./stability_for_analysis.tsv', sep='\t', index=None)
-            print("1:again, 2:hard, 3:good, 4:easy\n")
-            print(df[df['r_history'].str.contains(r'^[1-4][^124]*$', regex=True)][['r_history', 'avg_interval', 'avg_retention', 'stability', 'factor', 'group_cnt']].to_string(index=False))
             print("Analysis saved!")
+            caption = "1:again, 2:hard, 3:good, 4:easy\n"
+            analysis = df[df['r_history'].str.contains(r'^[1-4][^124]*$', regex=True)][['r_history', 'avg_interval', 'avg_retention', 'stability', 'factor', 'group_cnt']].to_string(index=False)
+            return caption + analysis
 
     def define_model(self):
         """Step 3"""
         self.init_w = [1, 1, 5, -0.5, -0.5, 0.2, 1.4, -0.2, 0.8, 2, -0.2, 0.2, 1]
         '''
         w[0]: initial_stability_for_again_answer
         w[1]: initial_stability_step_per_rating
@@ -471,33 +464,35 @@
         self.dataset = pd.read_csv("./revlog_history.tsv", sep='\t', index_col=None, dtype={'r_history': str ,'t_history': str} )
         self.dataset = self.dataset[(self.dataset['i'] > 1) & (self.dataset['delta_t'] > 0) & (self.dataset['t_history'].str.count(',0') == 0)]
         self.dataset['tensor'] = self.dataset.progress_apply(lambda x: lineToTensor(list(zip([x['t_history']], [x['r_history']]))[0]), axis=1)
         self.dataset['group'] = self.dataset['r_history'] + self.dataset['t_history']
         print("Tensorized!")
 
         w = []
+        plots = []
         if n_splits > 1:
             sgkf = StratifiedGroupKFold(n_splits=n_splits)
             for train_index, test_index in sgkf.split(self.dataset, self.dataset['i'], self.dataset['group']):
                 print("TRAIN:", len(train_index), "TEST:",  len(test_index))
                 train_set = self.dataset.iloc[train_index].copy()
                 test_set = self.dataset.iloc[test_index].copy()
                 trainer = Trainer(train_set, test_set, self.init_w, n_epoch=n_epoch, lr=lr, batch_size=batch_size)
                 w.append(trainer.train())
-                trainer.plot()
+                plots.append(trainer.plot())
         else:
             trainer = Trainer(self.dataset, self.dataset, self.init_w, n_epoch=n_epoch, lr=lr, batch_size=batch_size)
             w.append(trainer.train())
-            trainer.plot()
+            plots.append(trainer.plot())
 
         w = np.array(w)
         avg_w = np.round(np.mean(w, axis=0), 4)
         self.w = avg_w.tolist()
 
         print("\nTraining finished!")
+        return plots
 
     def preview(self, requestRetention: float):
         my_collection = Collection(self.w)
         print("1:again, 2:hard, 3:good, 4:easy\n")
         for first_rating in (1,2,3,4):
             print(f'first rating: {first_rating}')
             t_history = "0"
@@ -559,15 +554,15 @@
         self.difficulty_distribution = prediction.groupby(by=['difficulty'])['count'].sum() / prediction['count'].sum()
         print(self.difficulty_distribution)
         self.difficulty_distribution_padding = np.zeros(10)
         for i in range(10):
             if i+1 in self.difficulty_distribution.index:
                 self.difficulty_distribution_padding[i] = self.difficulty_distribution.loc[i+1]
     
-    def find_optimal_retention(self, graph=True):
+    def find_optimal_retention(self):
         """should not be called before predict_memory_states"""
 
         base = 1.01
         index_len = 664
         index_offset = 200
         d_range = 10
         d_offset = 1
@@ -610,15 +605,15 @@
                 return self.w[9] * np.power(d, self.w[10]) * np.power(s, self.w[11]) * np.exp((1 - r) * self.w[12])
 
 
         stability_list = np.array([np.power(base, i - index_offset) for i in range(index_len)])
         print(f"terminal stability: {stability_list.max(): .2f}")
         df = pd.DataFrame(columns=["retention", "difficulty", "time"])
 
-        for percentage in notebook.tqdm(range(96, 66, -2)):
+        for percentage in tqdm(range(96, 66, -2)):
             recall = percentage / 100
             time_list = np.zeros((d_range, index_len))
             time_list[:,:-1] = max_time
             for d in range(d_range, 0, -1):
                 s0 = init_stability(d)
                 s0_index = stability2index(s0)
                 diff = max_time
@@ -642,32 +637,33 @@
                 df.loc[0 if pd.isnull(df.index.max()) else df.index.max() + 1] = [recall, d, s0_time]
 
         df.sort_values(by=["difficulty", "retention"], inplace=True)
         df.to_csv("./expected_time.csv", index=False)
         print("expected_time.csv saved.")
 
         optimal_retention_list = np.zeros(10)
+        fig = plt.figure()
+        ax = fig.gca()
         for d in range(1, d_range+1):
             retention = df[df["difficulty"] == d]["retention"]
             cost = df[df["difficulty"] == d]["time"]
             optimal_retention = retention.iat[cost.argmin()]
             optimal_retention_list[d-1] = optimal_retention
-            plt.plot(retention, cost, label=f"d={d}, r={optimal_retention}")
+            ax.plot(retention, cost, label=f"d={d}, r={optimal_retention}")
         
         self.optimal_retention = np.inner(self.difficulty_distribution_padding, optimal_retention_list)
 
         print(f"\n-----suggested retention (experimental): {self.optimal_retention:.2f}-----")
 
-        if graph:
-            plt.ylabel("expected time (second)")
-            plt.xlabel("retention")
-            plt.legend()
-            plt.grid()
-            plt.semilogy()
-            plt.show()
+        ax.set_ylabel("expected time (second)")
+        ax.set_xlabel("retention")
+        ax.legend()
+        ax.grid()
+        ax.semilogy()
+        return (fig, )
     
     def evaluate(self):
         my_collection = Collection(self.init_w)
         stabilities, difficulties = my_collection.batch_predict(self.dataset)
         self.dataset['stability'] = stabilities
         self.dataset['difficulty'] = difficulties
         self.dataset['p'] = np.exp(np.log(0.9) * self.dataset['delta_t'] / self.dataset['stability'])
@@ -688,22 +684,21 @@
         tmp['p'] = tmp['p'].map(lambda x: round(x, 2))
         tmp['log_loss'] = tmp['log_loss'].map(lambda x: round(x, 2))
         tmp.rename(columns={"r": "grade", "p": "retrievability"}, inplace=True)
         tmp[['id', 'cid', 'review_date', 'r_history', 't_history', 'delta_t', 'grade', 'stability', 'difficulty', 'retrievability', 'log_loss']].to_csv("./evaluation.tsv", sep='\t', index=False)
         del tmp
 
     def calibration_graph(self):
-        plot_brier(self.dataset['p'], self.dataset['y'], bins=40)
-        plt.show()
+        fig1 = plot_brier(self.dataset['p'], self.dataset['y'], bins=40)
 
         def to_percent(temp, position):
             return '%1.0f' % (100 * temp) + '%'
 
-        fig = plt.figure(1)
-        ax1 = fig.add_subplot(111)
+        fig2 = plt.figure()
+        ax1 = fig2.add_subplot(111)
         ax2 = ax1.twinx()
         lns = []
 
         stability_calibration = pd.DataFrame(columns=['stability', 'predicted_retention', 'actual_retention'])
         stability_calibration = self.dataset[['stability', 'p', 'y']].copy()
         stability_calibration['bin'] = stability_calibration['stability'].map(lambda x: math.pow(1.2, math.floor(math.log(x, 1.2))))
         stability_group = stability_calibration.groupby('bin').count()
@@ -721,21 +716,20 @@
         ax2.set_ylabel("Retention")
         ax2.set_ylim(0, 1)
         lns.append(lns2[0])
         lns.append(lns3[0])
 
         labs = [l.get_label() for l in lns]
         ax2.legend(lns, labs, loc='lower right')
-        plt.grid(linestyle='--')
-        plt.gca().yaxis.set_major_formatter(ticker.FuncFormatter(to_percent))
-        plt.gca().xaxis.set_major_formatter(ticker.FormatStrFormatter('%d'))
-        plt.show()
+        ax2.grid(linestyle='--')
+        ax2.yaxis.set_major_formatter(ticker.FuncFormatter(to_percent))
+        ax2.xaxis.set_major_formatter(ticker.FormatStrFormatter('%d'))
 
-        fig = plt.figure(1)
-        ax1 = fig.add_subplot(111)
+        fig3 = plt.figure()
+        ax1 = fig3.add_subplot(111)
         ax2 = ax1.twinx()
         lns = []
 
         difficulty_calibration = pd.DataFrame(columns=['difficulty', 'predicted_retention', 'actual_retention'])
         difficulty_calibration = self.dataset[['difficulty', 'p', 'y']].copy()
         difficulty_calibration['bin'] = difficulty_calibration['difficulty'].map(round)
         difficulty_group = difficulty_calibration.groupby('bin').count()
@@ -752,18 +746,19 @@
         ax2.set_ylabel("Retention")
         ax2.set_ylim(0, 1)
         lns.append(lns2[0])
         lns.append(lns3[0])
 
         labs = [l.get_label() for l in lns]
         ax2.legend(lns, labs, loc='lower right')
-        plt.grid(linestyle='--')
-        plt.gca().yaxis.set_major_formatter(ticker.FuncFormatter(to_percent))
-        plt.gca().xaxis.set_major_formatter(ticker.FormatStrFormatter('%d'))
-        plt.show()
+        ax2.grid(linestyle='--')
+        ax2.yaxis.set_major_formatter(ticker.FuncFormatter(to_percent))
+        ax2.xaxis.set_major_formatter(ticker.FormatStrFormatter('%d'))
+
+        return fig1, fig2, fig3
 
     def bw_matrix(self):
         B_W_Metric_raw = self.dataset[['difficulty', 'stability', 'p', 'y']].copy()
         B_W_Metric_raw['s_bin'] = B_W_Metric_raw['stability'].map(lambda x: round(math.pow(1.4, math.floor(math.log(x, 1.4))), 2))
         B_W_Metric_raw['d_bin'] = B_W_Metric_raw['difficulty'].map(lambda x: int(round(x)))
         B_W_Metric = B_W_Metric_raw.groupby(by=['s_bin', 'd_bin']).agg('mean').reset_index()
         B_W_Metric_count = B_W_Metric_raw.groupby(by=['s_bin', 'd_bin']).agg('count').reset_index()
@@ -775,45 +770,46 @@
 
     def compare_with_sm2(self):
         self.dataset['sm2_ivl'] = self.dataset['tensor'].map(sm2)
         self.dataset['sm2_p'] = np.exp(np.log(0.9) * self.dataset['delta_t'] / self.dataset['sm2_ivl'])
         self.dataset['log_loss'] = self.dataset.apply(lambda row: - np.log(row['sm2_p']) if row['y'] == 1 else - np.log(1 - row['sm2_p']), axis=1)
         print(f"Loss of SM-2: {self.dataset['log_loss'].mean():.4f}")
         cross_comparison = self.dataset[['sm2_p', 'p', 'y']].copy()
-        plot_brier(cross_comparison['sm2_p'], cross_comparison['y'], bins=40)
+        fig1 = plot_brier(cross_comparison['sm2_p'], cross_comparison['y'], bins=40)
 
-        plt.figure(figsize=(6, 6))
+        fig2 = plt.figure(figsize=(6, 6))
+        ax = fig2.gca()
 
         cross_comparison['SM2_B-W'] = cross_comparison['sm2_p'] - cross_comparison['y']
         cross_comparison['SM2_bin'] = cross_comparison['sm2_p'].map(lambda x: round(x, 1))
         cross_comparison['FSRS_B-W'] = cross_comparison['p'] - cross_comparison['y']
         cross_comparison['FSRS_bin'] = cross_comparison['p'].map(lambda x: round(x, 1))
 
-        plt.axhline(y = 0.0, color = 'black', linestyle = '-')
+        ax.axhline(y = 0.0, color = 'black', linestyle = '-')
 
         cross_comparison_group = cross_comparison.groupby(by='SM2_bin').agg({'y': ['mean'], 'FSRS_B-W': ['mean'], 'p': ['mean', 'count']})
         print(f"Universal Metric of FSRS: {mean_squared_error(cross_comparison_group['y', 'mean'], cross_comparison_group['p', 'mean'], sample_weight=cross_comparison_group['p', 'count'], squared=False):.4f}")
         cross_comparison_group['p', 'percent'] = cross_comparison_group['p', 'count'] / cross_comparison_group['p', 'count'].sum()
-        plt.scatter(cross_comparison_group.index, cross_comparison_group['FSRS_B-W', 'mean'], s=cross_comparison_group['p', 'percent'] * 1024, alpha=0.5)
-        plt.plot(cross_comparison_group['FSRS_B-W', 'mean'], label='FSRS by SM2')
+        ax.scatter(cross_comparison_group.index, cross_comparison_group['FSRS_B-W', 'mean'], s=cross_comparison_group['p', 'percent'] * 1024, alpha=0.5)
+        ax.plot(cross_comparison_group['FSRS_B-W', 'mean'], label='FSRS by SM2')
 
         cross_comparison_group = cross_comparison.groupby(by='FSRS_bin').agg({'y': ['mean'], 'SM2_B-W': ['mean'], 'sm2_p': ['mean', 'count']})
         print(f"Universal Metric of SM2: {mean_squared_error(cross_comparison_group['y', 'mean'], cross_comparison_group['sm2_p', 'mean'], sample_weight=cross_comparison_group['sm2_p', 'count'], squared=False):.4f}")
         cross_comparison_group['sm2_p', 'percent'] = cross_comparison_group['sm2_p', 'count'] / cross_comparison_group['sm2_p', 'count'].sum()
-        plt.scatter(cross_comparison_group.index, cross_comparison_group['SM2_B-W', 'mean'], s=cross_comparison_group['sm2_p', 'percent'] * 1024, alpha=0.5)
-        plt.plot(cross_comparison_group['SM2_B-W', 'mean'], label='SM2 by FSRS')
+        ax.scatter(cross_comparison_group.index, cross_comparison_group['SM2_B-W', 'mean'], s=cross_comparison_group['sm2_p', 'percent'] * 1024, alpha=0.5)
+        ax.plot(cross_comparison_group['SM2_B-W', 'mean'], label='SM2 by FSRS')
 
-        plt.legend(loc='lower center')
-        plt.grid(linestyle='--')
-        plt.title("SM2 vs. FSRS")
-        plt.xlabel('Predicted R')
-        plt.ylabel('B-W Metric')
-        plt.xlim(0, 1)
-        plt.xticks(np.arange(0, 1.1, 0.1))
-        plt.show()
+        ax.legend(loc='lower center')
+        ax.grid(linestyle='--')
+        ax.set_title("SM2 vs. FSRS")
+        ax.set_xlabel('Predicted R')
+        ax.set_ylabel('B-W Metric')
+        ax.set_xlim(0, 1)
+        ax.set_xticks(np.arange(0, 1.1, 0.1))
+        return fig1, fig2
 
 # code from https://github.com/papousek/duolingo-halflife-regression/blob/master/evaluation.py
 def load_brier(predictions, real, bins=20):
     counts = np.zeros(bins)
     correct = np.zeros(bins)
     prediction = np.zeros(bins)
     for p, r in zip(predictions, real):
@@ -845,35 +841,36 @@
     bin_prediction_means = brier['detail']['bin_prediction_means']
     bin_correct_means = brier['detail']['bin_correct_means']
     bin_counts = brier['detail']['bin_counts']
     r2 = r2_score(bin_correct_means, bin_prediction_means, sample_weight=bin_counts)
     rmse = np.sqrt(mean_squared_error(bin_correct_means, bin_prediction_means, sample_weight=bin_counts))
     print(f"R-squared: {r2:.4f}")
     print(f"RMSE: {rmse:.4f}")
-    plt.figure()
-    ax = plt.gca()
-    ax.set_xlim([0, 1])
-    ax.set_ylim([0, 1])
-    plt.grid(True)
+    fig = plt.figure()
+    ax1 = fig.add_subplot(111)
+    ax1.set_xlim([0, 1])
+    ax1.set_ylim([0, 1])
+    ax1.grid(True)
     fit_wls = sm.WLS(bin_correct_means, sm.add_constant(bin_prediction_means), weights=bin_counts).fit()
     print(fit_wls.params)
     y_regression = [fit_wls.params[0] + fit_wls.params[1]*x for x in bin_prediction_means]
-    plt.plot(bin_prediction_means, y_regression, label='Weighted Least Squares Regression', color="green")
-    plt.plot(bin_prediction_means, bin_correct_means, label='Actual Calibration', color="#1f77b4")
-    plt.plot((0, 1), (0, 1), label='Perfect Calibration', color="#ff7f0e")
+    ax1.plot(bin_prediction_means, y_regression, label='Weighted Least Squares Regression', color="green")
+    ax1.plot(bin_prediction_means, bin_correct_means, label='Actual Calibration', color="#1f77b4")
+    ax1.plot((0, 1), (0, 1), label='Perfect Calibration', color="#ff7f0e")
     bin_count = brier['detail']['bin_count']
     counts = np.array(bin_counts)
     bins = (np.arange(bin_count) + 0.5) / bin_count
-    plt.legend(loc='upper center')
-    plt.xlabel('Predicted R')
-    plt.ylabel('Actual R')
-    plt.twinx()
-    plt.ylabel('Number of reviews')
-    plt.bar(bins, counts, width=(0.8 / bin_count), ec='k', lw=.2, alpha=0.5, label='Number of reviews')
-    plt.legend(loc='lower center')
+    ax1.legend(loc='upper center')
+    ax1.set_xlabel('Predicted R')
+    ax1.set_ylabel('Actual R')
+    ax2 = ax1.twinx()
+    ax2.set_ylabel('Number of reviews')
+    ax2.bar(bins, counts, width=(0.8 / bin_count), ec='k', lw=.2, alpha=0.5, label='Number of reviews')
+    ax2.legend(loc='lower center')
+    return fig
 
 def sm2(history):
     ivl = 0
     ef = 2.5
     reps = 0
     for delta_t, rating in history:
         delta_t = delta_t.item()
```

