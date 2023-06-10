# 부트 이미지 추출
# 내용확인
ls -la /dev/block/platform/soc/1d84000.ufshc/by-name   
# lrwxrwxrwx 1 root root   16 1970-03-30 00:29 boot -> /dev/block/sde45
# 추출
cat dev/block/sde45 > /data/local/tmp/myboot.img

# 파일가져오기
adb pull /data/local/tmp/myboot.img


# /data/local/tmp 폴더에서
dd if=/dev/block/bootdevice/by-name/boot of=./boot.img

# 마운트 RW로 다시하기
mount -o rw,remount /system

# 시스템을 추출
ls -la /dev/block/platform/soc/1d84000.ufshc/by-name   
# lrwxrwxrwx 1 root root   16 1970-04-02 09:01 system -> /dev/block/sde48

# 갤럭시
cat /dev/block/sda5 > /data/local/tmp/myboot.img   