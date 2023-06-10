# Comparing `tmp/nonebot_adapter_github-0.2.5.tar.gz` & `tmp/nonebot_adapter_github-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_github-0.2.5.tar", max compression
+gzip compressed data, was "nonebot_adapter_github-0.3.0.tar", max compression
```

## Comparing `nonebot_adapter_github-0.2.5.tar` & `nonebot_adapter_github-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1064 2022-12-05 14:57:33.089299 nonebot_adapter_github-0.2.5/LICENSE
--rw-r--r--   0        0        0     3829 2022-12-05 14:57:33.089299 nonebot_adapter_github-0.2.5/README.md
--rw-r--r--   0        0        0      543 2022-12-05 14:57:33.089299 nonebot_adapter_github-0.2.5/nonebot/adapters/github/__init__.py
--rw-r--r--   0        0        0     5322 2022-12-05 14:57:33.093299 nonebot_adapter_github-0.2.5/nonebot/adapters/github/adapter.py
--rw-r--r--   0        0        0     9542 2022-12-05 14:57:33.093299 nonebot_adapter_github-0.2.5/nonebot/adapters/github/bot.py
--rw-r--r--   0        0        0     1025 2022-12-05 14:57:33.093299 nonebot_adapter_github-0.2.5/nonebot/adapters/github/config.py
--rw-r--r--   0        0        0    47713 2022-12-05 14:57:33.093299 nonebot_adapter_github-0.2.5/nonebot/adapters/github/event.py
--rw-r--r--   0        0        0     1026 2022-12-05 14:57:33.093299 nonebot_adapter_github-0.2.5/nonebot/adapters/github/exception.py
--rw-r--r--   0        0        0     1153 2022-12-05 14:57:33.093299 nonebot_adapter_github-0.2.5/nonebot/adapters/github/message.py
--rw-r--r--   0        0        0      861 2022-12-05 14:57:33.093299 nonebot_adapter_github-0.2.5/nonebot/adapters/github/utils.py
--rw-r--r--   0        0        0     1320 2022-12-05 14:57:33.093299 nonebot_adapter_github-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     4695 1970-01-01 00:00:00.000000 nonebot_adapter_github-0.2.5/setup.py
--rw-r--r--   0        0        0     4927 1970-01-01 00:00:00.000000 nonebot_adapter_github-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-10 03:02:37.802700 nonebot_adapter_github-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3874 2023-06-10 03:02:37.802700 nonebot_adapter_github-0.3.0/README.md
+-rw-r--r--   0        0        0      543 2023-06-10 03:02:37.802700 nonebot_adapter_github-0.3.0/nonebot/adapters/github/__init__.py
+-rw-r--r--   0        0        0     5322 2023-06-10 03:02:37.802700 nonebot_adapter_github-0.3.0/nonebot/adapters/github/adapter.py
+-rw-r--r--   0        0        0     9653 2023-06-10 03:02:37.802700 nonebot_adapter_github-0.3.0/nonebot/adapters/github/bot.py
+-rw-r--r--   0        0        0     1025 2023-06-10 03:02:37.802700 nonebot_adapter_github-0.3.0/nonebot/adapters/github/config.py
+-rw-r--r--   0        0        0    51515 2023-06-10 03:02:37.806701 nonebot_adapter_github-0.3.0/nonebot/adapters/github/event.py
+-rw-r--r--   0        0        0     1026 2023-06-10 03:02:37.806701 nonebot_adapter_github-0.3.0/nonebot/adapters/github/exception.py
+-rw-r--r--   0        0        0     1153 2023-06-10 03:02:37.806701 nonebot_adapter_github-0.3.0/nonebot/adapters/github/message.py
+-rw-r--r--   0        0        0      861 2023-06-10 03:02:37.806701 nonebot_adapter_github-0.3.0/nonebot/adapters/github/utils.py
+-rw-r--r--   0        0        0     1383 2023-06-10 03:02:37.806701 nonebot_adapter_github-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4925 1970-01-01 00:00:00.000000 nonebot_adapter_github-0.3.0/PKG-INFO
```

### Comparing `nonebot_adapter_github-0.2.5/LICENSE` & `nonebot_adapter_github-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_github-0.2.5/README.md` & `nonebot_adapter_github-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <!-- markdownlint-disable-next-line MD041 -->
 <p align="center">
-  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
+  <a href="https://nonebot.dev/"><img src="https://raw.githubusercontent.com/nonebot/adapter-github/master/assets/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
 
 <div align="center">
 
 # NoneBot-Adapter-GitHub
 
 <!-- markdownlint-capture -->
```

### Comparing `nonebot_adapter_github-0.2.5/nonebot/adapters/github/__init__.py` & `nonebot_adapter_github-0.3.0/nonebot/adapters/github/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_github-0.2.5/nonebot/adapters/github/adapter.py` & `nonebot_adapter_github-0.3.0/nonebot/adapters/github/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_github-0.2.5/nonebot/adapters/github/bot.py` & `nonebot_adapter_github-0.3.0/nonebot/adapters/github/bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,31 @@
 from contextlib import asynccontextmanager
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     List,
     Union,
+    Generic,
+    TypeVar,
     Callable,
     Optional,
     AsyncGenerator,
 )
 
 from nonebot.typing import overrides
 from githubkit.utils import UNSET, Unset
 from nonebot.message import handle_event
-from githubkit import GitHub, AppAuthStrategy, TokenAuthStrategy, OAuthAppAuthStrategy
+from githubkit import (
+    GitHub,
+    AppAuthStrategy,
+    BaseAuthStrategy,
+    TokenAuthStrategy,
+    OAuthAppAuthStrategy,
+)
 
 from nonebot.adapters import Bot as BaseBot
 
 from .config import OAuthApp, GitHubApp
 from .message import Message, MessageSegment
 from .event import Event, CommitCommentCreated
 from .utils import APIContext, get_attr_or_item
@@ -28,14 +36,17 @@
 if TYPE_CHECKING:
     from githubkit.rest import RestNamespace
     from githubkit.rest.types import AppPermissionsType
 
     from .adapter import Adapter
 
 
+A = TypeVar("A", bound=BaseAuthStrategy)
+
+
 def _check_at_me(bot: "GitHubBot", event: Event) -> None:
     try:
         message = event.get_message()
     except Exception:
         return
 
     # ensure message not empty
@@ -109,15 +120,15 @@
         )
 
     raise RuntimeError(
         f"Cannot guess reply target for event type {event.__class__.__name__}"
     )
 
 
-class Bot(BaseBot):
+class Bot(BaseBot, Generic[A]):
     adapter: "Adapter"
 
     send_handler: Callable[
         ["Bot", Event, Union[str, Message, MessageSegment]], Any
     ] = send
 
     if TYPE_CHECKING:
@@ -128,15 +139,15 @@
         ) -> Dict[str, Any]:
             ...
 
     @overrides(BaseBot)
     def __init__(self, adapter: "Adapter", app: Union[GitHubApp, OAuthApp]):
         super().__init__(adapter, app.id)
         self.app = app
-        self._github: GitHub
+        self._github: GitHub[A]
         self._ctx_github: ContextVar[Optional[GitHub]] = ContextVar(
             "ctx_github", default=None
         )
 
     def __getattr__(self, name: str) -> APIContext:
         return APIContext(self, (name,))
 
@@ -150,19 +161,19 @@
     @overrides(BaseBot)
     async def send(
         self, event: Event, message: Union[str, Message, MessageSegment]
     ) -> Any:
         return await self.__class__.send_handler(self, event, message)
 
 
-class OAuthBot(Bot):
+class OAuthBot(Bot[OAuthAppAuthStrategy]):
     @overrides(Bot)
     def __init__(self, adapter: "Adapter", app: OAuthApp):
         super().__init__(adapter, app)
-        self._github: GitHub[OAuthAppAuthStrategy] = GitHub(
+        self._github = GitHub(
             OAuthAppAuthStrategy(app.client_id, app.client_secret),
             base_url=self.adapter.github_config.github_base_url,
             accept_format=self.adapter.github_config.github_accept_format,
             previews=self.adapter.github_config.github_previews,
             timeout=self.config.api_timeout,
         )
 
@@ -196,19 +207,19 @@
 
     @overrides(Bot)
     async def handle_event(self, event: Event) -> None:
         _check_nickname(self, event)
         await super().handle_event(event)
 
 
-class GitHubBot(Bot):
+class GitHubBot(Bot[AppAuthStrategy]):
     @overrides(Bot)
     def __init__(self, adapter: "Adapter", app: GitHubApp):
         super().__init__(adapter, app)
-        self._github: GitHub[AppAuthStrategy] = GitHub(
+        self._github = GitHub(
             AppAuthStrategy(
                 app.app_id, app.private_key, app.client_id, app.client_secret
             ),
             base_url=self.adapter.github_config.github_base_url,
             accept_format=self.adapter.github_config.github_accept_format,
             previews=self.adapter.github_config.github_previews,
             timeout=self.config.api_timeout,
```

### Comparing `nonebot_adapter_github-0.2.5/nonebot/adapters/github/config.py` & `nonebot_adapter_github-0.3.0/nonebot/adapters/github/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_github-0.2.5/nonebot/adapters/github/event.py` & `nonebot_adapter_github-0.3.0/nonebot/adapters/github/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,14 @@
 from githubkit.webhooks.models import MembershipRemoved as MembershipRemovedPayload
 from githubkit.webhooks.models import OrgBlockUnblocked as OrgBlockUnblockedPayload
 from githubkit.webhooks.models import ProjectCardEdited as ProjectCardEditedPayload
 from githubkit.webhooks.models import PullRequestClosed as PullRequestClosedPayload
 from githubkit.webhooks.models import PullRequestEdited as PullRequestEditedPayload
 from githubkit.webhooks.models import PullRequestLocked as PullRequestLockedPayload
 from githubkit.webhooks.models import PullRequestOpened as PullRequestOpenedPayload
-from githubkit.webhooks.models import PullRequestQueued as PullRequestQueuedPayload
 from githubkit.webhooks.models import RepositoryCreated as RepositoryCreatedPayload
 from githubkit.webhooks.models import RepositoryDeleted as RepositoryDeletedPayload
 from githubkit.webhooks.models import RepositoryRenamed as RepositoryRenamedPayload
 from githubkit.webhooks.models import SponsorshipEdited as SponsorshipEditedPayload
 from githubkit.webhooks.models import WorkflowJobQueued as WorkflowJobQueuedPayload
 from githubkit.webhooks.models import DiscussionAnswered as DiscussionAnsweredPayload
 from githubkit.webhooks.models import DiscussionUnlocked as DiscussionUnlockedPayload
@@ -95,34 +94,39 @@
 from githubkit.webhooks.models import ProjectCardDeleted as ProjectCardDeletedPayload
 from githubkit.webhooks.models import ProjectColumnMoved as ProjectColumnMovedPayload
 from githubkit.webhooks.models import PullRequestLabeled as PullRequestLabeledPayload
 from githubkit.webhooks.models import ReleasePrereleased as ReleasePrereleasedPayload
 from githubkit.webhooks.models import ReleaseUnpublished as ReleaseUnpublishedPayload
 from githubkit.webhooks.models import RepositoryArchived as RepositoryArchivedPayload
 from githubkit.webhooks.models import SponsorshipCreated as SponsorshipCreatedPayload
+from githubkit.webhooks.models import WorkflowJobWaiting as WorkflowJobWaitingPayload
 from githubkit.webhooks.models import CheckRunRerequested as CheckRunRerequestedPayload
 from githubkit.webhooks.models import CheckSuiteCompleted as CheckSuiteCompletedPayload
 from githubkit.webhooks.models import CheckSuiteRequested as CheckSuiteRequestedPayload
 from githubkit.webhooks.models import DiscussionUnlabeled as DiscussionUnlabeledPayload
 from githubkit.webhooks.models import InstallationCreated as InstallationCreatedPayload
 from githubkit.webhooks.models import InstallationDeleted as InstallationDeletedPayload
 from githubkit.webhooks.models import InstallationSuspend as InstallationSuspendPayload
 from githubkit.webhooks.models import IssueCommentCreated as IssueCommentCreatedPayload
 from githubkit.webhooks.models import IssueCommentDeleted as IssueCommentDeletedPayload
 from githubkit.webhooks.models import OrganizationDeleted as OrganizationDeletedPayload
 from githubkit.webhooks.models import OrganizationRenamed as OrganizationRenamedPayload
 from githubkit.webhooks.models import ProjectColumnEdited as ProjectColumnEditedPayload
 from githubkit.webhooks.models import PullRequestAssigned as PullRequestAssignedPayload
 from githubkit.webhooks.models import PullRequestDequeued as PullRequestDequeuedPayload
+from githubkit.webhooks.models import PullRequestEnqueued as PullRequestEnqueuedPayload
 from githubkit.webhooks.models import PullRequestReopened as PullRequestReopenedPayload
 from githubkit.webhooks.models import PullRequestUnlocked as PullRequestUnlockedPayload
 from githubkit.webhooks.models import (
     CommitCommentCreated as CommitCommentCreatedPayload,
 )
 from githubkit.webhooks.models import (
+    DependabotAlertFixed as DependabotAlertFixedPayload,
+)
+from githubkit.webhooks.models import (
     DiscussionUnanswered as DiscussionUnansweredPayload,
 )
 from githubkit.webhooks.models import (
     ProjectCardConverted as ProjectCardConvertedPayload,
 )
 from githubkit.webhooks.models import (
     ProjectColumnCreated as ProjectColumnCreatedPayload,
@@ -169,14 +173,17 @@
 from githubkit.webhooks.models import (
     ProjectsV2ItemCreated as ProjectsV2ItemCreatedPayload,
 )
 from githubkit.webhooks.models import (
     ProjectsV2ItemDeleted as ProjectsV2ItemDeletedPayload,
 )
 from githubkit.webhooks.models import (
+    PullRequestMilestoned as PullRequestMilestonedPayload,
+)
+from githubkit.webhooks.models import (
     PullRequestUnassigned as PullRequestUnassignedPayload,
 )
 from githubkit.webhooks.models import (
     RepositoryImportEvent as RepositoryImportEventPayload,
 )
 from githubkit.webhooks.models import (
     RepositoryTransferred as RepositoryTransferredPayload,
@@ -187,32 +194,44 @@
 from githubkit.webhooks.models import (
     WorkflowDispatchEvent as WorkflowDispatchEventPayload,
 )
 from githubkit.webhooks.models import (
     WorkflowJobInProgress as WorkflowJobInProgressPayload,
 )
 from githubkit.webhooks.models import (
+    WorkflowRunInProgress as WorkflowRunInProgressPayload,
+)
+from githubkit.webhooks.models import (
     CodeScanningAlertFixed as CodeScanningAlertFixedPayload,
 )
 from githubkit.webhooks.models import (
+    DependabotAlertCreated as DependabotAlertCreatedPayload,
+)
+from githubkit.webhooks.models import (
     ProjectsV2ItemArchived as ProjectsV2ItemArchivedPayload,
 )
 from githubkit.webhooks.models import (
     ProjectsV2ItemRestored as ProjectsV2ItemRestoredPayload,
 )
 from githubkit.webhooks.models import (
     PullRequestSynchronize as PullRequestSynchronizePayload,
 )
 from githubkit.webhooks.models import (
+    RegistryPackageUpdated as RegistryPackageUpdatedPayload,
+)
+from githubkit.webhooks.models import (
     SponsorshipTierChanged as SponsorshipTierChangedPayload,
 )
 from githubkit.webhooks.models import (
     CheckRunRequestedAction as CheckRunRequestedActionPayload,
 )
 from githubkit.webhooks.models import (
+    DependabotAlertReopened as DependabotAlertReopenedPayload,
+)
+from githubkit.webhooks.models import (
     DeploymentStatusCreated as DeploymentStatusCreatedPayload,
 )
 from githubkit.webhooks.models import (
     DiscussionCommentEdited as DiscussionCommentEditedPayload,
 )
 from githubkit.webhooks.models import (
     OrganizationMemberAdded as OrganizationMemberAddedPayload,
@@ -220,38 +239,50 @@
 from githubkit.webhooks.models import (
     ProjectsV2ItemConverted as ProjectsV2ItemConvertedPayload,
 )
 from githubkit.webhooks.models import (
     ProjectsV2ItemReordered as ProjectsV2ItemReorderedPayload,
 )
 from githubkit.webhooks.models import (
+    PullRequestDemilestoned as PullRequestDemilestonedPayload,
+)
+from githubkit.webhooks.models import (
     PullRequestReviewEdited as PullRequestReviewEditedPayload,
 )
 from githubkit.webhooks.models import (
     RepositoryDispatchEvent as RepositoryDispatchEventPayload,
 )
 from githubkit.webhooks.models import (
     SecurityAdvisoryUpdated as SecurityAdvisoryUpdatedPayload,
 )
 from githubkit.webhooks.models import (
     CodeScanningAlertCreated as CodeScanningAlertCreatedPayload,
 )
 from githubkit.webhooks.models import (
+    DependabotAlertDismissed as DependabotAlertDismissedPayload,
+)
+from githubkit.webhooks.models import (
     DiscussionCommentCreated as DiscussionCommentCreatedPayload,
 )
 from githubkit.webhooks.models import (
     DiscussionCommentDeleted as DiscussionCommentDeletedPayload,
 )
 from githubkit.webhooks.models import (
+    RegistryPackagePublished as RegistryPackagePublishedPayload,
+)
+from githubkit.webhooks.models import (
     CodeScanningAlertReopened as CodeScanningAlertReopenedPayload,
 )
 from githubkit.webhooks.models import (
     DiscussionCategoryChanged as DiscussionCategoryChangedPayload,
 )
 from githubkit.webhooks.models import (
+    InstallationTargetRenamed as InstallationTargetRenamedPayload,
+)
+from githubkit.webhooks.models import (
     MergeGroupChecksRequested as MergeGroupChecksRequestedPayload,
 )
 from githubkit.webhooks.models import (
     OrganizationMemberInvited as OrganizationMemberInvitedPayload,
 )
 from githubkit.webhooks.models import (
     OrganizationMemberRemoved as OrganizationMemberRemovedPayload,
@@ -283,20 +314,26 @@
 from githubkit.webhooks.models import (
     PullRequestReviewSubmitted as PullRequestReviewSubmittedPayload,
 )
 from githubkit.webhooks.models import (
     SecretScanningAlertCreated as SecretScanningAlertCreatedPayload,
 )
 from githubkit.webhooks.models import (
+    SecretScanningAlertRevoked as SecretScanningAlertRevokedPayload,
+)
+from githubkit.webhooks.models import (
     BranchProtectionRuleCreated as BranchProtectionRuleCreatedPayload,
 )
 from githubkit.webhooks.models import (
     BranchProtectionRuleDeleted as BranchProtectionRuleDeletedPayload,
 )
 from githubkit.webhooks.models import (
+    DependabotAlertReintroduced as DependabotAlertReintroducedPayload,
+)
+from githubkit.webhooks.models import (
     PullRequestAutoMergeEnabled as PullRequestAutoMergeEnabledPayload,
 )
 from githubkit.webhooks.models import (
     PullRequestConvertedToDraft as PullRequestConvertedToDraftPayload,
 )
 from githubkit.webhooks.models import (
     SecretScanningAlertReopened as SecretScanningAlertReopenedPayload,
@@ -353,26 +390,32 @@
 from githubkit.webhooks.models import (
     MarketplacePurchasePendingChange as MarketplacePurchasePendingChangePayload,
 )
 from githubkit.webhooks.models import (
     CodeScanningAlertAppearedInBranch as CodeScanningAlertAppearedInBranchPayload,
 )
 from githubkit.webhooks.models import (
+    DeploymentProtectionRuleRequested as DeploymentProtectionRuleRequestedPayload,
+)
+from githubkit.webhooks.models import (
     PullRequestReviewThreadUnresolved as PullRequestReviewThreadUnresolvedPayload,
 )
 from githubkit.webhooks.models import (
     InstallationNewPermissionsAccepted as InstallationNewPermissionsAcceptedPayload,
 )
 from githubkit.webhooks.models import (
     RepositoryVulnerabilityAlertCreate as RepositoryVulnerabilityAlertCreatePayload,
 )
 from githubkit.webhooks.models import (
     RepositoryVulnerabilityAlertReopen as RepositoryVulnerabilityAlertReopenPayload,
 )
 from githubkit.webhooks.models import (
+    SecretScanningAlertLocationCreated as SecretScanningAlertLocationCreatedPayload,
+)
+from githubkit.webhooks.models import (
     PullRequestReviewRequestRemovedOneof0,
     PullRequestReviewRequestRemovedOneof1,
 )
 from githubkit.webhooks.models import (
     RepositoryVulnerabilityAlertDismiss as RepositoryVulnerabilityAlertDismissPayload,
 )
 from githubkit.webhooks.models import (
@@ -573,26 +616,50 @@
     def get_message(self):
         return self._message
 
     class Config:
         keep_untouched = (cached_property,)
 
 
+class DependabotAlertCreated(Event):
+    payload: DependabotAlertCreatedPayload
+
+
+class DependabotAlertDismissed(Event):
+    payload: DependabotAlertDismissedPayload
+
+
+class DependabotAlertFixed(Event):
+    payload: DependabotAlertFixedPayload
+
+
+class DependabotAlertReintroduced(Event):
+    payload: DependabotAlertReintroducedPayload
+
+
+class DependabotAlertReopened(Event):
+    payload: DependabotAlertReopenedPayload
+
+
 class DeployKeyCreated(Event):
     payload: DeployKeyCreatedPayload
 
 
 class DeployKeyDeleted(Event):
     payload: DeployKeyDeletedPayload
 
 
 class DeploymentCreated(Event):
     payload: DeploymentCreatedPayload
 
 
+class DeploymentProtectionRuleRequested(Event):
+    payload: DeploymentProtectionRuleRequestedPayload
+
+
 class DeploymentStatusCreated(Event):
     payload: DeploymentStatusCreatedPayload
 
 
 class DiscussionAnswered(Event):
     payload: DiscussionAnsweredPayload
 
@@ -685,14 +752,18 @@
     payload: InstallationRepositoriesAddedPayload
 
 
 class InstallationRepositoriesRemoved(Event):
     payload: InstallationRepositoriesRemovedPayload
 
 
+class InstallationTargetRenamed(Event):
+    payload: InstallationTargetRenamedPayload
+
+
 class IssueCommentCreated(Event):
     payload: IssueCommentCreatedPayload
 
     @overrides(Event)
     def get_type(self) -> str:
         return "message"
 
@@ -1018,36 +1089,44 @@
     payload: PullRequestClosedPayload
 
 
 class PullRequestConvertedToDraft(Event):
     payload: PullRequestConvertedToDraftPayload
 
 
+class PullRequestDemilestoned(Event):
+    payload: PullRequestDemilestonedPayload
+
+
 class PullRequestDequeued(Event):
     payload: PullRequestDequeuedPayload
 
 
 class PullRequestEdited(Event):
     payload: PullRequestEditedPayload
 
 
+class PullRequestEnqueued(Event):
+    payload: PullRequestEnqueuedPayload
+
+
 class PullRequestLabeled(Event):
     payload: PullRequestLabeledPayload
 
 
 class PullRequestLocked(Event):
     payload: PullRequestLockedPayload
 
 
-class PullRequestOpened(Event):
-    payload: PullRequestOpenedPayload
+class PullRequestMilestoned(Event):
+    payload: PullRequestMilestonedPayload
 
 
-class PullRequestQueued(Event):
-    payload: PullRequestQueuedPayload
+class PullRequestOpened(Event):
+    payload: PullRequestOpenedPayload
 
 
 class PullRequestReadyForReview(Event):
     payload: PullRequestReadyForReviewPayload
 
 
 class PullRequestReopened(Event):
@@ -1145,14 +1224,22 @@
     payload: PullRequestReviewThreadResolvedPayload
 
 
 class PullRequestReviewThreadUnresolved(Event):
     payload: PullRequestReviewThreadUnresolvedPayload
 
 
+class RegistryPackagePublished(Event):
+    payload: RegistryPackagePublishedPayload
+
+
+class RegistryPackageUpdated(Event):
+    payload: RegistryPackageUpdatedPayload
+
+
 class ReleaseCreated(Event):
     payload: ReleaseCreatedPayload
 
 
 class ReleaseDeleted(Event):
     payload: ReleaseDeletedPayload
 
@@ -1237,14 +1324,22 @@
     payload: SecretScanningAlertReopenedPayload
 
 
 class SecretScanningAlertResolved(Event):
     payload: SecretScanningAlertResolvedPayload
 
 
+class SecretScanningAlertRevoked(Event):
+    payload: SecretScanningAlertRevokedPayload
+
+
+class SecretScanningAlertLocationCreated(Event):
+    payload: SecretScanningAlertLocationCreatedPayload
+
+
 class SecurityAdvisoryPerformed(Event):
     payload: SecurityAdvisoryPerformedPayload
 
 
 class SecurityAdvisoryPublished(Event):
     payload: SecurityAdvisoryPublishedPayload
 
@@ -1321,18 +1416,26 @@
     payload: WorkflowJobInProgressPayload
 
 
 class WorkflowJobQueued(Event):
     payload: WorkflowJobQueuedPayload
 
 
+class WorkflowJobWaiting(Event):
+    payload: WorkflowJobWaitingPayload
+
+
 class WorkflowRunCompleted(Event):
     payload: WorkflowRunCompletedPayload
 
 
+class WorkflowRunInProgress(Event):
+    payload: WorkflowRunInProgressPayload
+
+
 class WorkflowRunRequested(Event):
     payload: WorkflowRunRequestedPayload
 
 
 events = {
     "create": CreateEvent,
     "delete": DeleteEvent,
@@ -1370,21 +1473,31 @@
         "fixed": CodeScanningAlertFixed,
         "reopened": CodeScanningAlertReopened,
         "reopened_by_user": CodeScanningAlertReopenedByUser,
     },
     "commit_comment": {
         "created": CommitCommentCreated,
     },
+    "dependabot_alert": {
+        "created": DependabotAlertCreated,
+        "dismissed": DependabotAlertDismissed,
+        "fixed": DependabotAlertFixed,
+        "reintroduced": DependabotAlertReintroduced,
+        "reopened": DependabotAlertReopened,
+    },
     "deploy_key": {
         "created": DeployKeyCreated,
         "deleted": DeployKeyDeleted,
     },
     "deployment": {
         "created": DeploymentCreated,
     },
+    "deployment_protection_rule": {
+        "requested": DeploymentProtectionRuleRequested,
+    },
     "deployment_status": {
         "created": DeploymentStatusCreated,
     },
     "discussion": {
         "answered": DiscussionAnswered,
         "category_changed": DiscussionCategoryChanged,
         "created": DiscussionCreated,
@@ -1414,14 +1527,17 @@
         "suspend": InstallationSuspend,
         "unsuspend": InstallationUnsuspend,
     },
     "installation_repositories": {
         "added": InstallationRepositoriesAdded,
         "removed": InstallationRepositoriesRemoved,
     },
+    "installation_target": {
+        "renamed": InstallationTargetRenamed,
+    },
     "issue_comment": {
         "created": IssueCommentCreated,
         "deleted": IssueCommentDeleted,
         "edited": IssueCommentEdited,
     },
     "issues": {
         "assigned": IssuesAssigned,
@@ -1521,20 +1637,22 @@
     },
     "pull_request": {
         "assigned": PullRequestAssigned,
         "auto_merge_disabled": PullRequestAutoMergeDisabled,
         "auto_merge_enabled": PullRequestAutoMergeEnabled,
         "closed": PullRequestClosed,
         "converted_to_draft": PullRequestConvertedToDraft,
+        "demilestoned": PullRequestDemilestoned,
         "dequeued": PullRequestDequeued,
         "edited": PullRequestEdited,
+        "enqueued": PullRequestEnqueued,
         "labeled": PullRequestLabeled,
         "locked": PullRequestLocked,
+        "milestoned": PullRequestMilestoned,
         "opened": PullRequestOpened,
-        "queued": PullRequestQueued,
         "ready_for_review": PullRequestReadyForReview,
         "reopened": PullRequestReopened,
         "review_request_removed": PullRequestReviewRequestRemoved,
         "review_requested": PullRequestReviewRequested,
         "synchronize": PullRequestSynchronize,
         "unassigned": PullRequestUnassigned,
         "unlabeled": PullRequestUnlabeled,
@@ -1550,14 +1668,18 @@
         "deleted": PullRequestReviewCommentDeleted,
         "edited": PullRequestReviewCommentEdited,
     },
     "pull_request_review_thread": {
         "resolved": PullRequestReviewThreadResolved,
         "unresolved": PullRequestReviewThreadUnresolved,
     },
+    "registry_package": {
+        "published": RegistryPackagePublished,
+        "updated": RegistryPackageUpdated,
+    },
     "release": {
         "created": ReleaseCreated,
         "deleted": ReleaseDeleted,
         "edited": ReleaseEdited,
         "prereleased": ReleasePrereleased,
         "published": ReleasePublished,
         "released": ReleaseReleased,
@@ -1580,14 +1702,18 @@
         "reopen": RepositoryVulnerabilityAlertReopen,
         "resolve": RepositoryVulnerabilityAlertResolve,
     },
     "secret_scanning_alert": {
         "created": SecretScanningAlertCreated,
         "reopened": SecretScanningAlertReopened,
         "resolved": SecretScanningAlertResolved,
+        "revoked": SecretScanningAlertRevoked,
+    },
+    "secret_scanning_alert_location": {
+        "created": SecretScanningAlertLocationCreated,
     },
     "security_advisory": {
         "performed": SecurityAdvisoryPerformed,
         "published": SecurityAdvisoryPublished,
         "updated": SecurityAdvisoryUpdated,
         "withdrawn": SecurityAdvisoryWithdrawn,
     },
@@ -1613,13 +1739,15 @@
     "watch": {
         "started": WatchStarted,
     },
     "workflow_job": {
         "completed": WorkflowJobCompleted,
         "in_progress": WorkflowJobInProgress,
         "queued": WorkflowJobQueued,
+        "waiting": WorkflowJobWaiting,
     },
     "workflow_run": {
         "completed": WorkflowRunCompleted,
+        "in_progress": WorkflowRunInProgress,
         "requested": WorkflowRunRequested,
     },
 }
```

### Comparing `nonebot_adapter_github-0.2.5/nonebot/adapters/github/exception.py` & `nonebot_adapter_github-0.3.0/nonebot/adapters/github/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_github-0.2.5/nonebot/adapters/github/message.py` & `nonebot_adapter_github-0.3.0/nonebot/adapters/github/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_github-0.2.5/nonebot/adapters/github/utils.py` & `nonebot_adapter_github-0.3.0/nonebot/adapters/github/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_github-0.2.5/pyproject.toml` & `nonebot_adapter_github-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-github"
-version = "0.2.5"
+version = "0.3.0"
 description = "GitHub adapter for nonebot2"
 authors = ["yanyongyu <yyy@nonebot.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/nonebot/adapter-github"
 repository = "https://github.com/nonebot/adapter-github"
 documentation = "https://github.com/nonebot/adapter-github"
@@ -19,34 +19,39 @@
 packages = [
   { include = "nonebot" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nonebot2 = "^2.0.0-beta.5"
-githubkit = { version = ">=0.7.0,<1.0.0", extras = ["auth-app"] }
+githubkit = { version = ">=0.10.5,<1.0.0", extras = ["auth-app"] }
 
 [tool.poetry.group.dev.dependencies]
+pycln = "^2.1.4"
 isort = "^5.10.1"
-black = "^22.1.0"
+black = "^23.1.0"
 Jinja2 = "^3.1.2"
 nonemoji = "^0.1.2"
-pre-commit = "^2.20.0"
+pre-commit = "^3.1.0"
 
 [tool.black]
 line-length = 88
-target-version = ["py38", "py39", "py310"]
+target-version = ["py38", "py39", "py310", "py311"]
 include = '\.pyi?$'
 extend-exclude = '''
 '''
 
 [tool.isort]
 profile = "black"
 line_length = 88
 length_sort = true
 skip_gitignore = true
 force_sort_within_sections = true
 extra_standard_library = ["typing_extensions"]
 
+[tool.pycln]
+path = "."
+all = false
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_adapter_github-0.2.5/PKG-INFO` & `nonebot_adapter_github-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-github
-Version: 0.2.5
+Version: 0.3.0
 Summary: GitHub adapter for nonebot2
 Home-page: https://github.com/nonebot/adapter-github
 License: MIT
 Keywords: bot,github,webhook
 Author: yanyongyu
 Author-email: yyy@nonebot.dev
 Requires-Python: >=3.8,<4.0
@@ -14,24 +14,23 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Requires-Dist: githubkit[auth-app] (>=0.7.0,<1.0.0)
+Requires-Dist: githubkit[auth-app] (>=0.10.5,<1.0.0)
 Requires-Dist: nonebot2 (>=2.0.0-beta.5,<3.0.0)
 Project-URL: Documentation, https://github.com/nonebot/adapter-github
 Project-URL: Repository, https://github.com/nonebot/adapter-github
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable-next-line MD041 -->
 <p align="center">
-  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
+  <a href="https://nonebot.dev/"><img src="https://raw.githubusercontent.com/nonebot/adapter-github/master/assets/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
 
 <div align="center">
 
 # NoneBot-Adapter-GitHub
 
 <!-- markdownlint-capture -->
```

