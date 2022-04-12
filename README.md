Zoe Pratt (c) 2022

**DA:401 Senior Seminar in Data Analytics**
Final Capstone Project

This research analyzes the gameplay of eight top chess Grand Masters. To do so, unique style transfer generative adversarial networks (GANs) are created for each player. Then, the GAN models competed in a virtual chess tournament. Lastly, the accuracy of the GAN models was assessed.

**Data:** sourced from chess.com and ficsgames.org

**Code:** completed in Jupyter Notebooks and R.

The majority of the code files in this research are too computationally intense to be run on a local computer, so a remote Linux server was used. For ease of code review, I've included a Jupyter Notebook file titled **Model_Reproducible.ipynb** that uses condensed forms of the dataset (only 2 games from the PGN file) to extract the data, train 2 GAN models, and have them play against each other using condensed forms of the data. 

To run the code files in full (though not recommended on a local computer), the following order should be used:

**1:** All files in folder "Get_data". These parse through the PGN files provided and create numpy arrays for each chess board layout.

**2:** All files in folder "Create_models". These create a unique GAN model for each player

**3:** All files in folder "Tournaments", going in sequential order for the round (one, then two, then three). Here, the tournaments could potentially return different winners, so the GAN models used in subsequent tournaments would have to be altered.

**4**: Tournament analysis and GAN accuracy files (both .ipynb and .Rmd files) to analyze the winner's tournament play, as well as assess the overall accuracy of the GANs.
