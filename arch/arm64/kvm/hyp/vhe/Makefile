# SPDX-License-Identifier: GPL-2.0
#
# Makefile for Kernel-based Virtual Machine module, HYP/VHE part
#

asflags-y := -D__KVM_VHE_HYPERVISOR__
ccflags-y := -D__KVM_VHE_HYPERVISOR__

CFLAGS_switch.o += -Wno-override-init

obj-y := timer-sr.o sysreg-sr.o debug-sr.o switch.o tlb.o
obj-y += ../vgic-v3-sr.o ../aarch32.o ../vgic-v2-cpuif-proxy.o ../entry.o \
	 ../fpsimd.o ../hyp-entry.o ../exception.o
