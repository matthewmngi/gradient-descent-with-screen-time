# gradient-descent-with-screen-time

A simple gradient descent and cost function implementation on the screen time data and mental health risk scores of teenagers.

![Gradient descent results](/Figure_1.png)

## Setup
### Install dependencies

In your command line, run:

```
pip install -r requirements.txt
```
This will install all the dependencies.

---

### Load the dataset

These lines are near the top of `main.py`. They should execute when you run the file.

```
path = kagglehub.dataset_download("abdulmaliklodhra/social-media-impact-on-teen-behaviour-2015-2060", output_dir="./data", force_download=True)

print("Path to dataset files:", path)
```
*Note: After loading the dataset once, you can comment out these lines. The dataset only needs to be downloaded from Kaggle once.*

---

### Execution

The code should execute and display the following graph after running through the gradient descent function:

![Gradient descent results](/Figure_1.png)

I started with a learning rate of `1.0*e^-2`, but this proved to be inadequate. I've found that a learning rate of around `15` works best. A learning rate of 10 produces scalar errors.

---

### Next steps

You can modify the initialized `w` and `b` values, as well as the number of iterations and learning rate, to get a different result.