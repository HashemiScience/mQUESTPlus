# mQUESTPlus

## Introduction

mQuestPlus is a MATLAB implementation of Watson's QUEST+.

The method and Mathematica code are described in the paper:
Watson, A. B. (2017).  "QUEST+: A general multidimensional Bayesian adaptive psychometric method".
Journal of Vision, 17(3):10, 1-27.

This implementation follows quite closely the division into separate functions described in the paper
and illustrated in the Mathematica notebook.  The place to start is probably the demonstration/test
progams in the demos directory.  These reprise a number of figures in the Watson paper as well as
calculations illustrated by the Mathematica notebook that accompanies the paper.

Use "help mQuestPlus" at the Matlab prompt to access the contents of the package, and
then from you can click through to the routines in each subdirectory.

Similarly, "doc mQuestPlus" at the Matlab prompt will bring up the Matlab documentation viewer and
then you can click within that to explore the toolbox.

For each individual function, using "help qpRoutineName" or "doc qpRoutineName" will provide usage for that routine.

## Dependencies

This implementation depends on the following Matlab toolboxes:
  optimization -- used for fmincon numerical optimization routine in qpFit.
  stats -- used for computing things related to probability distributions.
The dependence on the stats toolbox could probably be worked around fairly easily.

For the circular distribution example, this toolbox depends on a toolbox that is free
from Matlab Central: 
  CircStat2012a -- used for von Mises distribution routines.  This is free from
    https://www.mathworks.com/matlabcentral/fileexchange/10676-circular-statistics-toolbox--directional-statistics-

## Installation

If you use our ToolboxToolbox (highly recommended, https://github.com/toolboxhub/ToolboxToolbox), simply type
"tbUse('mQuestPlus')" at the Matlab prompt to obtain mQuestPlus as well as CircStat2012a and put them onto your Matlab path.

Alternately, you can obtain mQuestPlus from https://github.com/brainardlab/mQuestPlus, either by cloning the
repository or by downloading and unpacking a zip file.  Then add it to your Matlab path.  If you want to run
the circular distribution example, obtain and add to your path CircStat2012a from Matlab Central at the URL
provided above.

## Known issues and bugs

See issues section of this (https://github.com/brainardlab/mQuestPlus) gitHub site for a list known issues,
limitations and possible future enhancements.  Please post an issue if you encounter a bug or wish to make
a suggestion.  We are happy to review and incorporate improvements and enhancements, either via gitHub pull
requests or if you just let us know via the issues or email (brainard@psych.upenn.edu).

## License 

mQuestPlus is released under the MIT open source license.

If you make use of the software in support of a publication, please cite it
(in addition to the Watson paper) as: Brainard, D. H. (2017) "mQuestPlus: A
Matlab implementation of QUEST+", https://github.com/brainardlab/mQuestPlus.

## Acknowledgments

This implementation is due to David Brainard.

Sources include the paper above, the Mathematica notebook provide as supplemental material for the paper
(an updated version of which was provided to me by Watson).

There is separate earlier Matlab implementation of QUEST+ written by P. R. Jones <petejonze@gmail.com>
in Joshua Soloman's laboratory.  The Jones implementation is organized differently from this one. Studying
it was useful, however, for thinking about ways to translate Mathematic data structures into Matlab.
The one place in the code where there was fairly direct carryover in data structure format is noted
specifically by comments in the code.

mQuestPlus includes allcomb.m, obtained from Matlab Central, along with its license.
  https://www.mathworks.com/matlabcentral/fileexchange/10064-allcomb-varargin-



