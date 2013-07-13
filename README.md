SpyderPandasPatch
=================

This is a quick dirty patch to Spyder, a great python GUI for data analysis, so that it supports the display of contents of  pandas Series and DataFrame

I feel excited about Spyder, which makes Python data analysis like Matlab. The only thing I find inconvinient is that the variable explorer does not support pandas Series and DataFrame in the current release (2.2.0). 

This is a very quick, simple, dirty patch to make it support the viewer for pd.Series, pd.DataFrame. But note that *** it does not support in place edit for pandas objects ***.

To apply the patch, if you are at Spyder 2.2.0, just copy two files from the /code to override the files Lib/site-packages/spyderlib/widgets/dicteditor.py and Lib/site-packages/spyderlib/widgets/dicteditorutils.py.

If you are not at Spyder 2.2.0, please see the reports in /report directory and make the changes by yourself. It is just several lines of changes. 

/snapshot directory gives you an idea how it will look like after applying this change.

