#
# CDDL HEADER START
#
# The contents of this file are subject to the terms of the
# Common Development and Distribution License (the License).
# You may not use this file except in compliance with the License.
#
# You can obtain a copy of the license at usr/src/CDDL.txt
# or http://www.opensolaris.org/os/licensing.
# See the License for the specific language governing permissions
# and limitations under the License.
#
# When distributing Covered Code, include this CDDL HEADER in each
# file and include the License file at usr/src/CDDL.txt.
# If applicable, add the following below this CDDL HEADER, with the
# fields enclosed by brackets [] replaced with your own identifying
# information: Portions Copyright [yyyy] [name of copyright owner]
#
# CDDL HEADER END
#
#
# Copyright 2007 Sun Microsystems, Inc.  All rights reserved.
# Use is subject to license terms.
#
# ident	"@(#)Makefile	1.6	07/04/19 SMI"
#
# Makefile for Files
#
# include global definitions
include ../Makefile.master
#

SUB_DIRS= \
		etc \
		lib \
		root \
		var

READ_FILES= \
		.cshrc \
		.profile

DIST_ROOT= ../$(ROOT)/Files

all install Files: $(READ_FILES) $(DIST_ROOT) $(READ_FILES:%=$(DIST_ROOT)/%) \
	$(SUB_DIRS)

top: $(READ_FILES) $(SUB_DIRS)

include ../Makefile.targs

clean clobber: $(SUB_DIRS) FRC

FRC:
