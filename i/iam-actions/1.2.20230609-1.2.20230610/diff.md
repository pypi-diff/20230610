# Comparing `tmp/iam_actions-1.2.20230609.tar.gz` & `tmp/iam_actions-1.2.20230610.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230609.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230610.tar", max compression
```

## Comparing `iam_actions-1.2.20230609.tar` & `iam_actions-1.2.20230610.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-06-09 02:50:52.839508 iam_actions-1.2.20230609/LICENSE
--rw-r--r--   0        0        0     2302 2023-06-09 02:50:52.839508 iam_actions-1.2.20230609/README.md
--rw-r--r--   0        0        0      228 2023-06-09 02:50:52.839508 iam_actions-1.2.20230609/iam_actions/__init__.py
--rw-r--r--   0        0        0  4300020 2023-06-09 02:52:29.188201 iam_actions-1.2.20230609/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-06-09 02:50:52.839508 iam_actions-1.2.20230609/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-06-09 02:50:52.839508 iam_actions-1.2.20230609/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-06-09 02:50:52.839508 iam_actions-1.2.20230609/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-06-09 02:50:52.839508 iam_actions-1.2.20230609/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-06-09 02:50:52.839508 iam_actions-1.2.20230609/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-06-09 02:50:52.839508 iam_actions-1.2.20230609/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-06-09 02:50:52.839508 iam_actions-1.2.20230609/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-06-09 02:50:52.839508 iam_actions-1.2.20230609/iam_actions/generate/services.py
--rw-r--r--   0        0        0   552817 2023-06-09 02:52:29.188201 iam_actions-1.2.20230609/iam_actions/policies.json
--rw-r--r--   0        0        0   196565 2023-06-09 02:52:29.188201 iam_actions-1.2.20230609/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   536179 2023-06-09 02:52:29.188201 iam_actions-1.2.20230609/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-06-09 02:52:29.944206 iam_actions-1.2.20230609/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230609/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230609/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-10 02:39:01.365870 iam_actions-1.2.20230610/LICENSE
+-rw-r--r--   0        0        0     2302 2023-06-10 02:39:01.365870 iam_actions-1.2.20230610/README.md
+-rw-r--r--   0        0        0      228 2023-06-10 02:39:01.365870 iam_actions-1.2.20230610/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4301381 2023-06-10 02:40:43.165764 iam_actions-1.2.20230610/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-06-10 02:39:01.365870 iam_actions-1.2.20230610/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-06-10 02:39:01.365870 iam_actions-1.2.20230610/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-06-10 02:39:01.365870 iam_actions-1.2.20230610/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-06-10 02:39:01.365870 iam_actions-1.2.20230610/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-06-10 02:39:01.365870 iam_actions-1.2.20230610/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-06-10 02:39:01.365870 iam_actions-1.2.20230610/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-06-10 02:39:01.365870 iam_actions-1.2.20230610/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-06-10 02:39:01.365870 iam_actions-1.2.20230610/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   552896 2023-06-10 02:40:43.165764 iam_actions-1.2.20230610/iam_actions/policies.json
+-rw-r--r--   0        0        0   195812 2023-06-10 02:40:43.165764 iam_actions-1.2.20230610/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   536255 2023-06-10 02:40:43.165764 iam_actions-1.2.20230610/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-06-10 02:40:43.973762 iam_actions-1.2.20230610/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230610/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230610/PKG-INFO
```

### Comparing `iam_actions-1.2.20230609/LICENSE` & `iam_actions-1.2.20230610/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230609/README.md` & `iam_actions-1.2.20230610/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230609/iam_actions/actions.json` & `iam_actions-1.2.20230610/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998004976624363%*

 * *Differences: {"'connect'": "{'SearchPrompts': OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *              "'SearchPrompts'), ('condition_keys', []), ('description', 'Not Documented by AWS'), "*

 * *              "('orphan', False), ('resources', [])]), 'SearchQuickConnects': "*

 * *              "OrderedDict([('access_level', 'Undocumented'), ('action', 'SearchQuickConnects'), "*

 * *              "('condition_keys', []), ('description', 'Not Documented by AWS'), ('orphan', "*

 * *              "False), ('resources', [])]), ' […]*

```diff
@@ -31509,27 +31509,51 @@
             "condition_keys": [],
             "description": "Grants permission to search phone number resources in an Amazon Connect instance or traffic distribution group",
             "orphan": false,
             "resources": [
                 "wildcard-phone-number"
             ]
         },
+        "SearchHoursOfOperations": {
+            "access_level": "Undocumented",
+            "action": "SearchHoursOfOperations",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "SearchPrompts": {
+            "access_level": "Undocumented",
+            "action": "SearchPrompts",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "SearchQueues": {
             "access_level": "Read",
             "action": "SearchQueues",
             "condition_keys": [
                 "connect:InstanceId",
                 "connect:SearchTag/${TagKey}"
             ],
             "description": "Grants permission to search queue resources in an Amazon Connect instance",
             "orphan": false,
             "resources": [
                 "instance"
             ]
         },
+        "SearchQuickConnects": {
+            "access_level": "Undocumented",
+            "action": "SearchQuickConnects",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "SearchRoutingProfiles": {
             "access_level": "Read",
             "action": "SearchRoutingProfiles",
             "condition_keys": [
                 "connect:InstanceId",
                 "connect:SearchTag/${TagKey}"
             ],
@@ -56015,280 +56039,280 @@
             "resources": [
                 "file-system"
             ]
         }
     },
     "elasticloadbalancing": {
         "AddListenerCertificates": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "AddListenerCertificates",
             "condition_keys": [],
-            "description": "Grants permission to add the specified certificates to the specified secure listener",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "listener/app",
-                "listener/net"
-            ]
+            "resources": []
         },
         "AddTags": {
             "access_level": "Tagging",
             "action": "AddTags",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "elasticloadbalancing:CreateAction",
+                "elasticloadbalancing:ResourceTag/${TagKey}"
             ],
             "description": "Grants permission to add the specified tags to the specified load balancer. Each load balancer can have a maximum of 10 tags",
             "orphan": false,
             "resources": [
-                "listener-rule/app",
-                "listener-rule/net",
-                "listener/app",
-                "listener/net",
-                "loadbalancer/app/",
-                "loadbalancer/net/",
-                "targetgroup"
+                "loadbalancer"
             ]
         },
         "ApplySecurityGroupsToLoadBalancer": {
             "access_level": "Write",
             "action": "ApplySecurityGroupsToLoadBalancer",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "elasticloadbalancing:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to associate one or more security groups with your load balancer in a virtual private cloud (VPC)",
             "orphan": false,
             "resources": [
                 "loadbalancer"
             ]
         },
         "AttachLoadBalancerToSubnets": {
             "access_level": "Write",
             "action": "AttachLoadBalancerToSubnets",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "elasticloadbalancing:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to add one or more subnets to the set of configured subnets for the specified load balancer",
             "orphan": false,
             "resources": [
                 "loadbalancer"
             ]
         },
         "ConfigureHealthCheck": {
             "access_level": "Write",
             "action": "ConfigureHealthCheck",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "elasticloadbalancing:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to specify the health check settings to use when evaluating the health state of your back-end instances",
             "orphan": false,
             "resources": [
                 "loadbalancer"
             ]
         },
         "CreateAppCookieStickinessPolicy": {
             "access_level": "Write",
             "action": "CreateAppCookieStickinessPolicy",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "elasticloadbalancing:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to generate a stickiness policy with sticky session lifetimes that follow that of an application-generated cookie",
             "orphan": false,
             "resources": [
                 "loadbalancer"
             ]
         },
         "CreateLBCookieStickinessPolicy": {
             "access_level": "Write",
             "action": "CreateLBCookieStickinessPolicy",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "elasticloadbalancing:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to generate a stickiness policy with sticky session lifetimes controlled by the lifetime of the browser (user-agent) or a specified expiration period",
             "orphan": false,
             "resources": [
                 "loadbalancer"
             ]
         },
         "CreateListener": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateListener",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to create a listener for the specified Application Load Balancer",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "loadbalancer/app/",
-                "loadbalancer/net/"
-            ]
+            "resources": []
         },
         "CreateLoadBalancer": {
             "access_level": "Write",
             "action": "CreateLoadBalancer",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "elasticloadbalancing:ResourceTag/${TagKey}"
             ],
             "description": "Grants permission to create a load balancer",
             "orphan": false,
             "resources": [
-                "loadbalancer/app/",
-                "loadbalancer/net/"
+                "loadbalancer"
             ]
         },
         "CreateLoadBalancerListeners": {
             "access_level": "Write",
             "action": "CreateLoadBalancerListeners",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "elasticloadbalancing:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to create one or more listeners for the specified load balancer",
             "orphan": false,
             "resources": [
                 "loadbalancer"
             ]
         },
         "CreateLoadBalancerPolicy": {
             "access_level": "Write",
             "action": "CreateLoadBalancerPolicy",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "elasticloadbalancing:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to create a policy with the specified attributes for the specified load balancer",
             "orphan": false,
             "resources": [
                 "loadbalancer"
             ]
         },
         "CreateRule": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateRule",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to create a rule for the specified listener",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "listener/app",
-                "listener/net"
-            ]
+            "resources": []
         },
         "CreateTargetGroup": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "CreateTargetGroup",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
-            "description": "Grants permission to create a target group",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "targetgroup"
-            ]
+            "resources": []
         },
         "DeleteListener": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteListener",
             "condition_keys": [],
-            "description": "Grants permission to delete the specified listener",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "listener/app",
-                "listener/net"
-            ]
+            "resources": []
         },
         "DeleteLoadBalancer": {
             "access_level": "Write",
             "action": "DeleteLoadBalancer",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "elasticloadbalancing:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to delete the specified load balancer",
             "orphan": false,
             "resources": [
-                "loadbalancer/app/",
-                "loadbalancer/net/"
+                "loadbalancer"
             ]
         },
         "DeleteLoadBalancerListeners": {
             "access_level": "Write",
             "action": "DeleteLoadBalancerListeners",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "elasticloadbalancing:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to delete the specified listeners from the specified load balancer",
             "orphan": false,
             "resources": [
                 "loadbalancer"
             ]
         },
         "DeleteLoadBalancerPolicy": {
             "access_level": "Write",
             "action": "DeleteLoadBalancerPolicy",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "elasticloadbalancing:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to delete the specified policy from the specified load balancer. This policy must not be enabled for any listeners",
             "orphan": false,
             "resources": [
                 "loadbalancer"
             ]
         },
         "DeleteRule": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteRule",
             "condition_keys": [],
-            "description": "Grants permission to delete the specified rule",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "listener-rule/app",
-                "listener-rule/net"
-            ]
+            "resources": []
         },
         "DeleteTargetGroup": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeleteTargetGroup",
             "condition_keys": [],
-            "description": "Grants permission to delete the specified target group",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "targetgroup"
-            ]
+            "resources": []
         },
         "DeregisterInstancesFromLoadBalancer": {
             "access_level": "Write",
             "action": "DeregisterInstancesFromLoadBalancer",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "elasticloadbalancing:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to deregister the specified instances from the specified load balancer",
             "orphan": false,
             "resources": [
                 "loadbalancer"
             ]
         },
         "DeregisterTargets": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "DeregisterTargets",
             "condition_keys": [],
-            "description": "Grants permission to deregister the specified targets from the specified target group",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "targetgroup"
-            ]
+            "resources": []
         },
         "DescribeAccountLimits": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "DescribeAccountLimits",
             "condition_keys": [],
-            "description": "Grants permission to describe the Elastic Load Balancing resource limits for the AWS account",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeInstanceHealth": {
             "access_level": "Read",
             "action": "DescribeInstanceHealth",
             "condition_keys": [],
             "description": "Grants permission to describe the state of the specified instances with respect to the specified load balancer",
             "orphan": false,
             "resources": []
         },
         "DescribeListenerCertificates": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "DescribeListenerCertificates",
             "condition_keys": [],
-            "description": "Grants permission to describe the certificates for the specified secure listener",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeListeners": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "DescribeListeners",
             "condition_keys": [],
-            "description": "Grants permission to describe the specified listeners or the listeners for the specified Application Load Balancer",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeLoadBalancerAttributes": {
             "access_level": "Read",
             "action": "DescribeLoadBalancerAttributes",
             "condition_keys": [],
@@ -56309,281 +56333,273 @@
             "action": "DescribeLoadBalancerPolicyTypes",
             "condition_keys": [],
             "description": "Grants permission to describe the specified load balancer policy types",
             "orphan": false,
             "resources": []
         },
         "DescribeLoadBalancers": {
-            "access_level": "Read",
+            "access_level": "List",
             "action": "DescribeLoadBalancers",
             "condition_keys": [],
             "description": "Grants permission to describe the specified the load balancers. If no load balancers are specified, the call describes all of your load balancers",
             "orphan": false,
             "resources": []
         },
         "DescribeRules": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "DescribeRules",
             "condition_keys": [],
-            "description": "Grants permission to describe the specified rules or the rules for the specified listener",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeSSLPolicies": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "DescribeSSLPolicies",
             "condition_keys": [],
-            "description": "Grants permission to describe the specified policies or all policies used for SSL negotiation",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeTags": {
             "access_level": "Read",
             "action": "DescribeTags",
             "condition_keys": [],
-            "description": "Grants permission to describe the tags associated with the specified resource",
+            "description": "Grants permission to describe the tags associated with the specified load balancers",
             "orphan": false,
             "resources": []
         },
         "DescribeTargetGroupAttributes": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "DescribeTargetGroupAttributes",
             "condition_keys": [],
-            "description": "Grants permission to describe the attributes for the specified target group",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeTargetGroups": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "DescribeTargetGroups",
             "condition_keys": [],
-            "description": "Grants permission to describe the specified target groups or all of your target groups",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeTargetHealth": {
-            "access_level": "Read",
+            "access_level": "Undocumented",
             "action": "DescribeTargetHealth",
             "condition_keys": [],
-            "description": "Grants permission to describe the health of the specified targets or all of your targets",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DetachLoadBalancerFromSubnets": {
             "access_level": "Write",
             "action": "DetachLoadBalancerFromSubnets",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "elasticloadbalancing:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to remove the specified subnets from the set of configured subnets for the load balancer",
             "orphan": false,
             "resources": [
                 "loadbalancer"
             ]
         },
         "DisableAvailabilityZonesForLoadBalancer": {
             "access_level": "Write",
             "action": "DisableAvailabilityZonesForLoadBalancer",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "elasticloadbalancing:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to remove the specified Availability Zones from the set of Availability Zones for the specified load balancer",
             "orphan": false,
             "resources": [
                 "loadbalancer"
             ]
         },
         "EnableAvailabilityZonesForLoadBalancer": {
             "access_level": "Write",
             "action": "EnableAvailabilityZonesForLoadBalancer",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "elasticloadbalancing:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to add the specified Availability Zones to the set of Availability Zones for the specified load balancer",
             "orphan": false,
             "resources": [
                 "loadbalancer"
             ]
         },
         "ModifyListener": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyListener",
             "condition_keys": [],
-            "description": "Grants permission to modify the specified properties of the specified listener",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "listener/app",
-                "listener/net"
-            ]
+            "resources": []
         },
         "ModifyLoadBalancerAttributes": {
             "access_level": "Write",
             "action": "ModifyLoadBalancerAttributes",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "elasticloadbalancing:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to modify the attributes of the specified load balancer",
             "orphan": false,
             "resources": [
-                "loadbalancer/app/",
-                "loadbalancer/net/"
+                "loadbalancer"
             ]
         },
         "ModifyRule": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyRule",
             "condition_keys": [],
-            "description": "Grants permission to modify the specified rule",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "listener-rule/app",
-                "listener-rule/net"
-            ]
+            "resources": []
         },
         "ModifyTargetGroup": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyTargetGroup",
             "condition_keys": [],
-            "description": "Grants permission to modify the health checks used when evaluating the health state of the targets in the specified target group",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "targetgroup"
-            ]
+            "resources": []
         },
         "ModifyTargetGroupAttributes": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "ModifyTargetGroupAttributes",
             "condition_keys": [],
-            "description": "Grants permission to modify the specified attributes of the specified target group",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "targetgroup"
-            ]
+            "resources": []
         },
         "RegisterInstancesWithLoadBalancer": {
             "access_level": "Write",
             "action": "RegisterInstancesWithLoadBalancer",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "elasticloadbalancing:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to add the specified instances to the specified load balancer",
             "orphan": false,
             "resources": [
                 "loadbalancer"
             ]
         },
         "RegisterTargets": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RegisterTargets",
             "condition_keys": [],
-            "description": "Grants permission to register the specified targets with the specified target group",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "targetgroup"
-            ]
+            "resources": []
         },
         "RemoveListenerCertificates": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "RemoveListenerCertificates",
             "condition_keys": [],
-            "description": "Grants permission to remove the specified certificates of the specified secure listener",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "listener/app",
-                "listener/net"
-            ]
+            "resources": []
         },
         "RemoveTags": {
             "access_level": "Tagging",
             "action": "RemoveTags",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "elasticloadbalancing:ResourceTag/${TagKey}"
             ],
             "description": "Grants permission to remove one or more tags from the specified load balancer",
             "orphan": false,
             "resources": [
-                "listener-rule/app",
-                "listener-rule/net",
-                "listener/app",
-                "listener/net",
-                "loadbalancer/app/",
-                "loadbalancer/net/",
-                "targetgroup"
+                "loadbalancer"
             ]
         },
         "SetIpAddressType": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "SetIpAddressType",
             "condition_keys": [],
-            "description": "Grants permission to set the type of IP addresses used by the subnets of the specified load balancer",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "loadbalancer/app/",
-                "loadbalancer/net/"
-            ]
+            "resources": []
         },
         "SetLoadBalancerListenerSSLCertificate": {
             "access_level": "Write",
             "action": "SetLoadBalancerListenerSSLCertificate",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "elasticloadbalancing:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to set the certificate that terminates the specified listener's SSL connections",
             "orphan": false,
             "resources": [
                 "loadbalancer"
             ]
         },
         "SetLoadBalancerPoliciesForBackendServer": {
             "access_level": "Write",
             "action": "SetLoadBalancerPoliciesForBackendServer",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "elasticloadbalancing:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to replace the set of policies associated with the specified port on which the back-end server is listening with a new set of policies",
             "orphan": false,
             "resources": [
                 "loadbalancer"
             ]
         },
         "SetLoadBalancerPoliciesOfListener": {
             "access_level": "Write",
             "action": "SetLoadBalancerPoliciesOfListener",
-            "condition_keys": [],
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "elasticloadbalancing:ResourceTag/${TagKey}"
+            ],
             "description": "Grants permission to replace the current set of policies for the specified load balancer port with the specified set of policies",
             "orphan": false,
             "resources": [
                 "loadbalancer"
             ]
         },
         "SetRulePriorities": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "SetRulePriorities",
             "condition_keys": [],
-            "description": "Grants permission to set the priorities of the specified rules",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "listener-rule/app",
-                "listener-rule/net"
-            ]
+            "resources": []
         },
         "SetSecurityGroups": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "SetSecurityGroups",
             "condition_keys": [],
-            "description": "Grants permission to associate the specified security groups with the specified load balancer",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "loadbalancer/app/",
-                "loadbalancer/net/"
-            ]
+            "resources": []
         },
         "SetSubnets": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "SetSubnets",
             "condition_keys": [],
-            "description": "Grants permission to enable the Availability Zone for the specified subnets for the specified load balancer",
+            "description": "Not Documented by AWS",
             "orphan": false,
-            "resources": [
-                "loadbalancer/app/",
-                "loadbalancer/net/"
-            ]
+            "resources": []
         },
         "SetWebAcl": {
-            "access_level": "Write",
+            "access_level": "Undocumented",
             "action": "SetWebAcl",
             "condition_keys": [],
-            "description": "Grants permission to give WebAcl permission to WAF",
+            "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "elasticmapreduce": {
         "AddInstanceFleet": {
             "access_level": "Write",
@@ -107678,20 +107694,26 @@
             "description": "Grants permission to add a profile key",
             "orphan": false,
             "resources": [
                 "domains"
             ]
         },
         "CreateCalculatedAttributeDefinition": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateCalculatedAttributeDefinition",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to create a calculated attribute definition in the domain",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "calculated-attributes",
+                "domains"
+            ]
         },
         "CreateDomain": {
             "access_level": "Write",
             "action": "CreateDomain",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
@@ -107699,20 +107721,26 @@
             "description": "Grants permission to create a Domain",
             "orphan": false,
             "resources": [
                 "domains"
             ]
         },
         "CreateEventStream": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateEventStream",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to put an event stream in a domain",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "domains",
+                "event-streams"
+            ]
         },
         "CreateIntegrationWorkflow": {
             "access_level": "Write",
             "action": "CreateIntegrationWorkflow",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
@@ -107730,38 +107758,44 @@
             "description": "Grants permission to create a profile in the domain",
             "orphan": false,
             "resources": [
                 "domains"
             ]
         },
         "DeleteCalculatedAttributeDefinition": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteCalculatedAttributeDefinition",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete a calculated attribute definition in the domain",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "calculated-attributes",
+                "domains"
+            ]
         },
         "DeleteDomain": {
             "access_level": "Write",
             "action": "DeleteDomain",
             "condition_keys": [],
             "description": "Grants permission to delete a Domain",
             "orphan": false,
             "resources": [
                 "domains"
             ]
         },
         "DeleteEventStream": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteEventStream",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete an event stream in a domain",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "domains",
+                "event-streams"
+            ]
         },
         "DeleteIntegration": {
             "access_level": "Write",
             "action": "DeleteIntegration",
             "condition_keys": [],
             "description": "Grants permission to delete a integration in a domain",
             "orphan": false,
@@ -107829,46 +107863,55 @@
             "description": "Grants permission to get a preview of auto merging in a domain",
             "orphan": false,
             "resources": [
                 "domains"
             ]
         },
         "GetCalculatedAttributeDefinition": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetCalculatedAttributeDefinition",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to get a calculated attribute definition in the domain",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "calculated-attributes",
+                "domains"
+            ]
         },
         "GetCalculatedAttributeForProfile": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetCalculatedAttributeForProfile",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to retrieve a calculated attribute for a specific profile in the domain",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "calculated-attributes",
+                "domains"
+            ]
         },
         "GetDomain": {
             "access_level": "Read",
             "action": "GetDomain",
             "condition_keys": [],
             "description": "Grants permission to get a specific domain in an account",
             "orphan": false,
             "resources": [
                 "domains"
             ]
         },
         "GetEventStream": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetEventStream",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to get a specific event stream in a domain",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "domains",
+                "event-streams"
+            ]
         },
         "GetIdentityResolutionJob": {
             "access_level": "Read",
             "action": "GetIdentityResolutionJob",
             "condition_keys": [],
             "description": "Grants permission to get an identity resolution job in a domain",
             "orphan": false,
@@ -107941,44 +107984,50 @@
             "action": "ListAccountIntegrations",
             "condition_keys": [],
             "description": "Grants permission to list all the integrations in the account",
             "orphan": false,
             "resources": []
         },
         "ListCalculatedAttributeDefinitions": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListCalculatedAttributeDefinitions",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list all the calculated attribute definitions in the domain",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "domains"
+            ]
         },
         "ListCalculatedAttributesForProfile": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListCalculatedAttributesForProfile",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list all calculated attributes for a specific profile in the domain",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "domains"
+            ]
         },
         "ListDomains": {
             "access_level": "List",
             "action": "ListDomains",
             "condition_keys": [],
             "description": "Grants permission to list all the domains in an account",
             "orphan": false,
             "resources": []
         },
         "ListEventStreams": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListEventStreams",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list all the event streams in a specific domain",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "domains"
+            ]
         },
         "ListIdentityResolutionJobs": {
             "access_level": "List",
             "action": "ListIdentityResolutionJobs",
             "condition_keys": [],
             "description": "Grants permission to list identity resolution jobs in a domain",
             "orphan": false,
@@ -108027,15 +108076,21 @@
         },
         "ListTagsForResource": {
             "access_level": "Read",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Grants permission to list tags for a resource",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "calculated-attributes",
+                "domains",
+                "event-streams",
+                "integrations",
+                "object-types"
+            ]
         },
         "ListWorkflows": {
             "access_level": "List",
             "action": "ListWorkflows",
             "condition_keys": [],
             "description": "Grants permission to list all the workflows in a specific domain",
             "orphan": false,
@@ -108107,34 +108162,49 @@
             "action": "TagResource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to adds tags to a resource",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "calculated-attributes",
+                "domains",
+                "event-streams",
+                "integrations",
+                "object-types"
+            ]
         },
         "UntagResource": {
             "access_level": "Tagging",
             "action": "UntagResource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to remove tags from a resource",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "calculated-attributes",
+                "domains",
+                "event-streams",
+                "integrations",
+                "object-types"
+            ]
         },
         "UpdateCalculatedAttributeDefinition": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateCalculatedAttributeDefinition",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update a calculated attribute definition in the domain",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "calculated-attributes",
+                "domains"
+            ]
         },
         "UpdateDomain": {
             "access_level": "Write",
             "action": "UpdateDomain",
             "condition_keys": [],
             "description": "Grants permission to update a Domain",
             "orphan": false,
@@ -137210,20 +137280,22 @@
             "description": "Grants permission to a queue for a specific principal",
             "orphan": false,
             "resources": [
                 "queue"
             ]
         },
         "CancelMessageMoveTask": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CancelMessageMoveTask",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to cancel an in progress message move task",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "queue"
+            ]
         },
         "ChangeMessageVisibility": {
             "access_level": "Write",
             "action": "ChangeMessageVisibility",
             "condition_keys": [],
             "description": "Grants permission to change the visibility timeout of a specified message in a queue to a new value",
             "orphan": false,
@@ -137291,20 +137363,22 @@
             "description": "Grants permission to return a list of your queues that have the RedrivePolicy queue attribute configured with a dead letter queue",
             "orphan": false,
             "resources": [
                 "queue"
             ]
         },
         "ListMessageMoveTasks": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "ListMessageMoveTasks",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list message move tasks",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "queue"
+            ]
         },
         "ListQueueTags": {
             "access_level": "Read",
             "action": "ListQueueTags",
             "condition_keys": [],
             "description": "Grants permission to list tags added to an SQS queue",
             "orphan": false,
@@ -137367,20 +137441,22 @@
             "description": "Grants permission to set the value of one or more queue attributes",
             "orphan": false,
             "resources": [
                 "queue"
             ]
         },
         "StartMessageMoveTask": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StartMessageMoveTask",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to start a message move task",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "queue"
+            ]
         },
         "TagQueue": {
             "access_level": "Tagging",
             "action": "TagQueue",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
```

### Comparing `iam_actions-1.2.20230609/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230610/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230609/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230610/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230609/iam_actions/generate/generate.py` & `iam_actions-1.2.20230610/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230609/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230610/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230609/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230610/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230609/iam_actions/generate/services.py` & `iam_actions-1.2.20230610/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230609/iam_actions/policies.json` & `iam_actions-1.2.20230610/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999998358589174%*

 * *Differences: {"'serviceMap'": "{'Amazon Connect': {'Actions': {insert: [(139, 'SearchHoursOfOperations'), (140, "*

 * *                 "'SearchPrompts'), (142, 'SearchQuickConnects')]}}}"}*

```diff
@@ -11542,15 +11542,18 @@
                 "ListUsers",
                 "MonitorContact",
                 "PutUserStatus",
                 "ReleasePhoneNumber",
                 "ReplicateInstance",
                 "ResumeContactRecording",
                 "SearchAvailablePhoneNumbers",
+                "SearchHoursOfOperations",
+                "SearchPrompts",
                 "SearchQueues",
+                "SearchQuickConnects",
                 "SearchRoutingProfiles",
                 "SearchSecurityProfiles",
                 "SearchUsers",
                 "SearchVocabularies",
                 "StartChatContact",
                 "StartContactEvaluation",
                 "StartContactRecording",
```

### Comparing `iam_actions-1.2.20230609/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230610/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982291666666667%*

 * *Differences: {"'elasticloadbalancing'": "{delete: ['listener/app', 'listener-rule/app', 'listener/net', "*

 * *                           "'listener-rule/net', 'loadbalancer/app/', 'loadbalancer/net/', "*

 * *                           "'targetgroup']}",*

 * * "'profile'": "{'event-streams': OrderedDict([('arn_pattern', "*

 * *              "'arn:*:profile:*:*:domains/*/event-streams/*'), ('condition_keys', "*

 * *              "'aws:ResourceTag/${TagKey}')]), 'calculated-attributes': "*

 * *              "OrderedDict([('arn_pattern', "*

 * *             […]*

```diff
@@ -2405,45 +2405,17 @@
         },
         "file-system": {
             "arn_pattern": "arn:*:elasticfilesystem:*:*:file-system/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "elasticloadbalancing": {
-        "listener-rule/app": {
-            "arn_pattern": "arn:*:elasticloadbalancing:*:*:listener-rule/app/*/*/*/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        },
-        "listener-rule/net": {
-            "arn_pattern": "arn:*:elasticloadbalancing:*:*:listener-rule/net/*/*/*/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        },
-        "listener/app": {
-            "arn_pattern": "arn:*:elasticloadbalancing:*:*:listener/app/*/*/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        },
-        "listener/net": {
-            "arn_pattern": "arn:*:elasticloadbalancing:*:*:listener/net/*/*/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        },
         "loadbalancer": {
             "arn_pattern": "arn:*:elasticloadbalancing:*:*:loadbalancer/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
-        },
-        "loadbalancer/app/": {
-            "arn_pattern": "arn:*:elasticloadbalancing:*:*:loadbalancer/app/*/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        },
-        "loadbalancer/net/": {
-            "arn_pattern": "arn:*:elasticloadbalancing:*:*:loadbalancer/net/*/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
-        },
-        "targetgroup": {
-            "arn_pattern": "arn:*:elasticloadbalancing:*:*:targetgroup/*/*",
-            "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "elasticmapreduce": {
         "cluster": {
             "arn_pattern": "arn:*:elasticmapreduce:*:*:cluster/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
@@ -4826,18 +4798,26 @@
         },
         "order": {
             "arn_pattern": "arn:*:private-networks:*:*:order/*/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "profile": {
+        "calculated-attributes": {
+            "arn_pattern": "arn:*:profile:*:*:domains/*/calculated-attributes/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
         "domains": {
             "arn_pattern": "arn:*:profile:*:*:domains/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
+        "event-streams": {
+            "arn_pattern": "arn:*:profile:*:*:domains/*/event-streams/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
         "integrations": {
             "arn_pattern": "arn:*:profile:*:*:domains/*/integrations/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "object-types": {
             "arn_pattern": "arn:*:profile:*:*:domains/*/object-types/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
```

### Comparing `iam_actions-1.2.20230609/iam_actions/services.json` & `iam_actions-1.2.20230610/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999982810781078%*

 * *Differences: {"'connect'": "{'Actions': {insert: [(139, 'SearchHoursOfOperations'), (140, 'SearchPrompts'), "*

 * *              "(142, 'SearchQuickConnects')]}}"}*

```diff
@@ -4685,15 +4685,18 @@
             "ListUsers",
             "MonitorContact",
             "PutUserStatus",
             "ReleasePhoneNumber",
             "ReplicateInstance",
             "ResumeContactRecording",
             "SearchAvailablePhoneNumbers",
+            "SearchHoursOfOperations",
+            "SearchPrompts",
             "SearchQueues",
+            "SearchQuickConnects",
             "SearchRoutingProfiles",
             "SearchSecurityProfiles",
             "SearchUsers",
             "SearchVocabularies",
             "StartChatContact",
             "StartContactEvaluation",
             "StartContactRecording",
```

### Comparing `iam_actions-1.2.20230609/pyproject.toml` & `iam_actions-1.2.20230610/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230609"
+version = "1.2.20230610"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230609/setup.py` & `iam_actions-1.2.20230610/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230609',
+    'version': '1.2.20230610',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230609/PKG-INFO` & `iam_actions-1.2.20230610/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230609
+Version: 1.2.20230610
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

