
.PHONY: px4-dev-armhf, px4-dev-base-archlinux, px4-dev-base-bionic, \
		px4-dev-base-xenial, px4-dev-clang, px4-dev-nuttx, \
		px4-dev-nuttx-clang, px4-dev-raspi, px4-dev-ros-kinetic, \
		px4-dev-ros-melodic, px4-dev-ros2-ardent, px4-dev-ros2-bouncy, \
		px4-dev-ros2-crystal, px4-dev-ros2-dashing, px4-dev-ros2-eloquent, \
		px4-dev-simulation-xenial, px4-dev-simulation-bionic

all: px4-dev-armhf, px4-dev-base-archlinux, px4-dev-base-bionic, \
		px4-dev-base-xenial, px4-dev-clang, px4-dev-nuttx, \
		px4-dev-nuttx-clang, px4-dev-raspi, px4-dev-ros-kinetic, \
		px4-dev-ros-melodic, px4-dev-ros2-ardent, px4-dev-ros2-bouncy, \
		px4-dev-ros2-crystal, px4-dev-ros2-dashing, px4-dev-ros2-eloquent, \
		px4-dev-simulation-xenial, px4-dev-simulation-bionic

px4-dev-armhf:
	docker build -t px4io/px4-dev-armhf . -f Dockerfile_armhf

px4-dev-base-archlinux:
	docker build -t px4io/px4-dev-base-archlinux . -f Dockerfile_base-archlinux

px4-dev-base-bionic:
	docker build -t px4io/px4-dev-base-bionic . -f Dockerfile_base-bionic

px4-dev-base-xenial:
	docker build -t px4io/px4-dev-base-xenial . -f Dockerfile_base-xenial

px4-dev-clang: px4-dev-base-bionic
	docker build -t px4io/px4-dev-clang . -f Dockerfile_clang

px4-dev-nuttx: px4-dev-base-bionic
	docker build -t px4io/px4-dev-nuttx . -f Dockerfile_nuttx

px4-dev-nuttx-clang: px4-dev-clang
	docker build -t px4io/px4-dev-nuttx-clang . -f Dockerfile_nuttx_clang

px4-dev-raspi: px4-dev-base-bionic
	docker build -t px4io/px4-dev-raspi . -f Dockerfile_raspi

px4-dev-ros-kinetic: px4-dev-simulation-xenial
	docker build -t px4io/px4-dev-ros-kinetic . -f Dockerfile_ros-kinetic

px4-dev-ros-melodic: px4-dev-simulation-bionic
	docker build -t px4io/px4-dev-ros-melodic . -f Dockerfile_ros-melodic

px4-dev-ros2-ardent: px4-dev-ros-kinetic
	docker build -t px4io/px4-dev-ros2-ardent . -f Dockerfile_ros2-ardent

px4-dev-ros2-bouncy: px4-dev-ros-melodic
	docker build -t px4io/px4-dev-ros2-bouncy . -f Dockerfile_ros2-bouncy

px4-dev-ros2-crystal: px4-dev-ros-melodic
	docker build -t px4io/px4-dev-ros2-crystal . -f Dockerfile_ros2-crystal

px4-dev-ros2-bouncy: px4-dev-ros-melodic
	docker build -t px4io/px4-dev-ros2-bouncy . -f Dockerfile_ros2-bouncy

px4-dev-ros2-dashing: px4-dev-ros-melodic
	docker build -t px4io/px4-dev-ros2-dashing . -f Dockerfile_ros2-dashing

px4-dev-ros2-eloquent: px4-dev-ros-melodic
	docker build -t px4io/px4-dev-ros2-eloquent . -f Dockerfile_ros2-eloquent

px4-dev-simulation-xenial: px4-dev-base-xenial
	docker build -t px4io/px4-dev-simulation-xenial . -f Dockerfile_simulation-xenial

px4-dev-simulation-bionic: px4-dev-base-bionic
	docker build -t px4io/px4-dev-simulation-bionic . -f Dockerfile_simulation-bionic
