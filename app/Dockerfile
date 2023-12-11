FROM --platform=linux/riscv64 busybox AS image
COPY ./init /init

# squash
FROM --platform=linux/riscv64 scratch
COPY --from=image / /
CMD sh /init
