# Function To Draw Vectors

This tool samples a math function and turns it into plotter commands.

## Files

- `draw_math.py` - main script
- `output/` - sample generated graph command files
  
## Run

```bash
python src/draw_math.py "sin(x)" --xmin -3.14159 --xmax 3.14159 --samples 200 --width-mm 40 --height-mm 40
```

Included sample outputs:

- `graph_sin_x_.txt`
- `graph_cos_x_.txt`
- `graph_x__3.txt`
