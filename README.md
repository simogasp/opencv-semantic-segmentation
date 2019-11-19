To enable python opencv

```bash
export PYTHONPATH=$PYTHONPATH:<opencv_install_path>/lib/python2.7/dist-packages
```

For a single image:

```bash
python segment.py --model enet-cityscapes/enet-model.net \
	--classes enet-cityscapes/enet-classes.txt \
	--colors enet-cityscapes/enet-colors.txt \
	--image images/example_04.png
```

For a video:

```bash
python segment_video.py --model enet-cityscapes/enet-model.net \
	--classes enet-cityscapes/enet-classes.txt \
	--colors enet-cityscapes/enet-colors.txt \
	--video videos/massachusetts.mp4 \
	--output output/massachusetts_output.avi
```