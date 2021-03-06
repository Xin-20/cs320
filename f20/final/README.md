# Final "Exam"

For the final "exam", you'll do a mini project on a dataset of your
choosing.  You'll practice supervised and unsupervised learning,
create three plots, and write one page of text.

You must do the work independently, but you can seek feedback,
debugging, and proofreading help from any other 320 students, as long
as they are not working on the same dataset as you.  Cite anybody
(besides 320 staff) who helps you.

**Due Date:** Dec 15th (when the 320 exam is scheduled in student center), by the end of the day.  We encourage you to start earlier, of course.

## Clarifications/Corrections

* Dec 3: complete example added below

## Specifications

You'll produce a 2-page PDF using your tool of choice.  For example,
you could use Microsoft Word, then export to PDF.  The second page of
your PDF will contain exactly three figures (nothing else).  The first
page will, among other things, describe those figures.

### Figures (Page 2)

You'll create three figures (options/requirements for each below).
Set a title for each figure that includes the figure number, like
this: `ax.set_title("Figure 1: ????", pad=20)`.

When you copy/paste the figures to the document, make sure they don't
get stretched/distorted.  It's best to set font size and figsize in
matplotlib to get the sizing correct.  Any text on the figures should
be close in size to the text on the second page of your document.
Visually verify this in the final PDF before you submit. When you set
the font size in matplotlib, then save to an image that gets copied to
the document, the resulting figure text may look smaller than you
expected.

Axis labels should be specific ("quantity" is not a descriptive
label).  Avoid misleading axis limits (not starting from 0 often makes
differences appear more dramatic than reality).

#### Figure 1: descriptive stats

You have a lot of flexibility for what to include for this one.  The
main requirement is that you visually communicate more than 2
dimensions of the data.  **Options:**

1. stacked bar plot
2. clustered bar plot
3. line plot with multiple lines
4. scatter plot (a geographic map with points on it counts).  Either shape, size, or color of points must communicate a third dimension of the data beyond what is already communicated by the x-axis and y-axis

Make sure you choose the right plot design for your data (don't use a
line plot if your x-axis is categorical, for example).

#### Figure 2: unsupervised ML

Use either sklearn KMeans or PCA on some subset of your data.  You are
encouraged to consider doing so as part of an sklearn pipeline
(StandardScaler or PolynomialFeatures might be useful, for example).

Your figure should communicate something about your KMeans or PCA
results.  **Options:**

1. scatter plot, where color and/or shape shows clusters (KMeans over 2 dimensions)
2. line plot, where x-axis is number of clusters and y-axis is inertia (KMeans with any number of dimensions)
3. scatter plot, where x-axis and y-axis show the first two principal components (PCA that reduces to 2 dimensions)
4. line plot, where x-axis is number of components and y-axis is cumulative explained variance (PCA with any number of dimensions)

#### Figure 3: supervised ML

Use either sklearn LinearRegression or LogisticRegression to predict
some column of your dataset (as for Figure 2, you're encouraged to do
so as part of an sklearn pipeline).  Your figure should communicate
something about your results.  **Options:**

1. line(s) fit to some scatter data (LinearRegression correlating two variables)
2. scatter plot with points showing actual class of row over contourf that shows decision boundaries (LogisticRegression doing prediction based on two input variables)
3. bar plot showing coefficients (LinearRegression or LogisticRegression)

### Text (Page 1)

The quality of your text is very important to your grade.  Read this
essay by venture capitalist Paul Graham on useful writing before you
get started: http://www.paulgraham.com/useful.html.

You should introduce and motivate your project: what questions do
you hope to answer, and why do they matter?  Satisfying curiosity
generally isn't enough motivation.  If you can, be specific about how
your work will inform a policy or help somebody make a better
decision.

Describe your dataset.  Where/how did you get it (a hyperlink is
appropriate in most cases)?  Obtaining data via web scraping, taking
measurements, or combining multiple datasets from multiple sources is
encouraged.  Using pre-cleaned datasets (from kaggle, for example) is
discouraged.  Don't list actual column names here; instead, describe
the kinds of information available and what you'll use.

Write a paragraph or two for each of your figures.  Reference the
figure number in the text (for example, you might say "Figure 1 shows
...").  Include text that helps one read the plot (for example, "each
point represents ...") and that makes observations (for example, "we
see that ...").

Be quantitative.  Instead of "we see a positive relationship between
____ and ____", actually say what the slope/formula is in the text.
Good text is full of simple, memorable statistics (percents, averages,
etc.).  Some of these will relate to what can be seen in the figures,
and others should refer to other analysis you did.

Don't include code examples, but write in a way that another
programmer could roughly reproduce your results.  What
cleanup/transformations did you do on the data?  What stages were
there in your sklearn pipelines?  Why did you choose those stages?
You're encouraged to justify your decisions by quantifying improvement
over worse versions you tried.

Your text should fill the whole page (or at least be close); it must
not go over.  Use font size between 10 and 14, single spaced, with
margins roughly 1 inch.  Do not include bulleted lists.  If anybody
helped you (for example, with proofreading) besides 320 staff, briefly
thank them by name at the end of your text.  Strive to be concise,
complete, and (grammatically) correct.  Do a spellcheck before
submitting.

## Complete Example

See [Water Breaks in Madison](example.pdf) for a complete example of a
final project.

Thanks to Wen Ye (320 mentor), Gautam Agarwal, and Bryan Jin for
providing the inspiration for this example (the three of them have
been working together on a far more comprehensive version of this
study).

## Submission and Grading

Details coming soon...