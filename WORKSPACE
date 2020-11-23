#  Copyright 2020 Northwestern Inclusive Technology Lab
# 
#  Licensed under the Apache License, Version 2.0 (the "License");
#  you may not use this file except in compliance with the License.
#  You may obtain a copy of the License at
# 
#     http://www.apache.org/licenses/LICENSE-2.0
# 
#  Unless required by applicable law or agreed to in writing, software
#  distributed under the License is distributed on an "AS IS" BASIS,
#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
#  See the License for the specific language governing permissions and
#  limitations under the License.

workspace(
    name = "rules_node_addon"
)

#####################################################
### Import Required Repo and URL Management Tools ###
#####################################################

load("@bazel_tools//tools/build_defs/repo:git.bzl", "git_repository")

###########################################
### Define URL and keys for build rules ###
###########################################

# C++ Build Rules
rules_cc_repo_url = "https://github.com/bazelbuild/rules_cc.git"
rules_cc_commit_latest = "b1c40e1de81913a3c40e5948f78719c28152486d"

###################################
### Retrieve Rules From Sources ###
###################################

# C++ Build Rules
# LICENSE: The Apache Software License, Version 2.0
git_repository(
    name = "rules_cc",
    remote = rules_cc_repo_url,
    init_submodules = True,
    commit = rules_cc_commit_latest
)

##############################################
### Load & Customize Retrieved Build Rules ###
##############################################
