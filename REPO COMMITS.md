# Command to get the total lines of code contributed by each author in the repository
git log --all --pretty='%an <%ae>' --numstat | awk '
  $0 ~ /<[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}>$/ { author = $0; sub(/.* </, "<", author); next }
  /^[0-9-]+[[:space:]]+[0-9-]+[[:space:]]+/ {
    if ($1 != "-") added += $1
    if ($2 != "-") deleted += $2
    lines[author] += added + deleted
    added = deleted = 0
  }
  END {
    total = 0
    for (a in lines) total += lines[a]
    if (total == 0) { print "No lines tracked — repo might have binary files or bad history"; exit }
    print "Total tracked lines (added + modified): " total
    print "──────────────────────────────────────────────"
    for (a in lines) {
      perc = lines[a] / total * 100
      printf "%.2f%%  %8d lines  %s\n", perc, lines[a], a
    }
  }' | sort -nr

factiii.com
  58.33%   1465940 lines  <jsnyder10@gmail.com>
11.18%    280988 lines  <hm754831@gmail.com>
8.19%    205929 lines  <89443652+parik36@users.noreply.github.com>
7.75%    194734 lines  <90836930+AmnaZahoor11@users.noreply.github.com>
6.64%    166773 lines  <yashgouravkar@gmail.com>
5.79%    145516 lines  <72254541+Hammad69275@users.noreply.github.com>
1.19%     29996 lines  <parik36@icloud.com>
0.74%     18698 lines  <144723498+devhuzaiffa@users.noreply.github.com>
0.18%      4595 lines  <29817246+saketsarin@users.noreply.github.com>
Total tracked lines (added + modified): 2513233
0.00%        64 lines  <devhammad2@gmail.com>

greasemoto.com
90.14%   1842624 lines  <jsnyder10@gmail.com>
7.56%    154568 lines  <sarinsaket@gmail.com>
2.17%     44425 lines  <hm754831@gmail.com>
0.12%      2472 lines  <shubhhampgit02@gmail.com>
0.01%       117 lines  <162743085+RealBusinessInc@users.noreply.github.com>
Total tracked lines (added + modified): 2044206

link3d.io
83.27%    436166 lines  <jsnyder10@gmail.com>
16.73%     87638 lines  <hm754831@gmail.com>
Total tracked lines (added + modified): 523804

taptrack.io
66.88%    232037 lines  <jsnyder10@gmail.com>
18.00%     62452 lines  <farhan.asghar@softcircles.org>
7.77%     26949 lines  <bdsolar.solutions@gmail.com>
4.36%     15134 lines  <carter@link3d.io>
2.99%     10363 lines  <hm754831@gmail.com>
Total tracked lines (added + modified): 346935
