#homework 2

mkdir fsd_HW2;

knot 0;
git init;
emacs README.md (add "#homework 2");
git add README.md;
git commit -m "Initial commit";


knot 1;
emacs README.md  (add "First edit");
git add README.md;
git commit -m "First commit";


knot 2;
emacs README.md  (add "Second edit");
git add README.md;
git commit -m "Second commit";


knot 3;
git log (to see the version number of Initial Commit at knot 0);
git checkout  0edc9e6b8803e93b8cc7555db62df9a6f8ad02c7;
git checkout -b bug-fix;
emacs README.md  (add "Third edit");
git add README.md;
git commit -m "Thrid commit";


knot 4;
emacs README.md  (add "Forth edit");
git add README.md;
git commit -m "Forth commit";


knot 5;
git checkout master;
git log (to see the version number of Second Commit at knot 2);
git checkout bug-fix;
git merge 206638f3396ee6ce2803dfe8eb378be5bfb1f6b7;
emacs README.md (remove useless words );
git add README.md;
git commit -m "Fifth Commit-Fixed Conflict";


knot 6;
emacs README.md (add "Fifth edit");
git add README.md;
git commit -m "Sixth Commit";


knot 7;
git log (to see the version number of Forth Commit at knot 4);
git checkout f234c51a3b3e1eb3abd17912ea41d7da60c081cf;
git checkout -b bug-fix-experimental;
emacs README.md (add "Sixth edit");
git add README.md;
git commit -m "Seventh Commit";


knot 8;
emacs README.md (add "Seventh edit");
git add README.md;
git commit -m "Eighth Commit";



knot 9;
emacs README.md (add "Eighth edit");
git add README.md;
git commit -m "Ninth Commit";


knot 10;
git checkout master;
emacs README.md (add "Ninth edit");
git add README.md;
git commit -m "Tenth Commit";


knot 11;
git checkout bug-fix-experimental;
git log (to see the version number of Ninth commit knot 9);
git checkout bug-fix;
git merge 79f0823d3f46eb4c9d999d1e96aeb702fe4a0078 (merge to knot 9);
emacs README.md (remove useless words);
git add README.md;
git commit -m "Eleventh Commit-Fixed Conflict 2";


knot 12;
emacs README.md (add "Tenth edit");
git add README.md;
git commit -m "Twelfth Commit";


knot 13;
git log (to see the version number of 12th commit at knot 12);
git checkout master;
git merge a997748f731abb65b4d3cd55fefe6a3aee22d330;
emacs README.md (remove useless words);
git add README.md;
git commit -m "Thirteenth Commit-Fixed conflict 3";


knot 14;
emacs README.md (add all previous command );
git add README.md;
git commit -m "Fourteenth Commit";
