# Running

Set up [uv](https://docs.astral.sh/uv/) aka run `pip install uv`

Then ensure you save the data of the "bones obj files" in `/data/bones obj files`

In the same way as in the original repo, adjust these parameters when you want to change which scan to run.

The only difference here is that I added 'device' which allows you to explicitly pick the folder where to find the scan data.

```
# process more files
multi_files = False
index_default = 1
# switch for figure
show_figure = False
bone_type = Bone.Type.FEMUR
device: Literal["bones obj files", "iphone_ten", "structure_sensor", "cubic box obj files", "bones_combined", "starbucks_cup"] = "starbucks_cup"
```

Data was retrieved and calculated by hand from /web/out/core_alg/results and comparing to the ground truth data.
