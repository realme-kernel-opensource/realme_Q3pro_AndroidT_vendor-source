obj-y += sched_assist_common.o
obj-y += sched_assist_mutex.o
obj-y += sched_assist_rwsem.o
obj-y += sched_assist_futex.o
obj-y += sched_assist_workqueue.o
obj-y += sched_assist_rt.o
obj-$(CONFIG_LOCKING_PROTECT) += sched_assist_locking.o

#qcom
ifeq ($(CONFIG_OPLUS_SYSTEM_KERNEL_QCOM), y)
ifeq ($(VERSION).$(PATCHLEVEL), 5.4)
obj-y += sched_assist_slide.o
endif
#mtk
else
obj-$(CONFIG_SCHED_WALT) += sched_assist_slide_v1.o
endif
