#
# Licensed to the Apache Software Foundation (ASF) under one
# or more contributor license agreements. See the NOTICE file
# distributed with this work for additional information
# regarding copyright ownership. The ASF licenses this file
# to you under the Apache License, Version 2.0 (the
# "License"); you may not use this file except in compliance
# with the License. You may obtain a copy of the License at
#
#   http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing,
# software distributed under the License is distributed on an
# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
# KIND, either express or implied. See the License for the
# specific language governing permissions and limitations
# under the License.
#

EXTRA_DIST = \
  README \
  Setup.lhs \
  TODO \
  Thrift.cabal \
  src

all-local:
	$(RUNHASKELL) Setup.lhs configure $(CABAL_CONFIGURE_FLAGS)
	$(RUNHASKELL) Setup.lhs build

install-exec-hook:
	$(RUNHASKELL) Setup.lhs install

# Make sure this doesn't fail if Haskell is not configured.
clean-local:
	$(RUNHASKELL) Setup.lhs clean

maintainer-clean-local:
	$(RUNHASKELL) Setup.lhs clean
