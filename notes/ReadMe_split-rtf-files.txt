# https://ss64.com/mac/split.html

# split them like this
split -b 10m windowsToGoDocs.rtf windowsToGoDocs.rtf_
split -b 10m windowsToGoDocs\ 4.rtf windowsToGoDocs\ 4.rtf_

# re-assemble them like this
cat `ls windowsToGoDocs.rtf_*` > windowsToGoDocs.rtf
cat `ls windowsToGoDocs\ 4.rtf_*` > windowsToGoDocs\ 4.rtf

