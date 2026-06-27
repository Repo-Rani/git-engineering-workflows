Class-1

Install git and github
we have a tow types of repo in this 
1) git local repo
2) github remote repo

1) configuration for connect git with your github account:
git config --global user.name "Write Here UserName From Github Account"

2) configure you git email with the same github account email:
git config --global user.email "Write Here same Email From Github Account"

3) Git Configuration List Command is
git config --list

class-2

1) To push your working directory do these steps one by one:
step-1: create repositry in a github Web Host
step-2: git init (For git initialization in a working dircetory ) 
step-3: git add file name or . (For tracking changes of files / or Maintain History Of These Files)
step-4: git commit -m "Write Here Message for Commit" (To store code in a local git repositry)
step-5: git branch -M main (For main Branch / By default Github branch name is main/ for Branch name Rename)
step-6: git remote add origin "Url for Github repo" (To push working dir in a remote repositry/ Origin: It is a short and easy nickname (alias) for a long GitHub repository URL, so you don't have to type the whole address every time)
step-7: git push origin -u main (To push code in a remote repo/ -u To async local branch from remote branch)

class-3 

1) Repositry?
   repositry ek a si storage location hoti he jaha par hum apne code ko or us ki history ko maintain krte hn. (code me kab kaha kis line me kiya changes ki he us ko history bolte hn) . repo ka kam hmri working dir k changes ko track krna hota he

2) Working Directory?
   working dirctory ek a si location hoti he jaha par hum apne code ko likh rhe hote hein ya us par work kr rhe hote hn.jis mei hum apni development kr rhe hote he.(is dir me changes krne se hmri git me changes hi hoti hume manually commands k throw git me add krna hota he..WD me jab tak hum git init nhi krte he tab tak git track nhi kr skta he)  

3) Local Repository?
   ap ki repo ka wo version jo ap k computer me locally saved ho rha hota he.(is ko is liye banate hn takay hum apne code kis history ko dekh sake or commit kr sake.. ye hmre code k version,histroycode ki changes ko store or change krwane k liye local repo create krte hn . throw the git init command)

4) Remote Repository?
   A si Repository jaha par ap apne code ko store to krwte ho magr ya Hosting plateforms par banti hn.(code ko share ya collaborate kr skte hn. You also say its Global Repository)      

Git Workflow
                     git add .                                    git commit -m                  git push
working directory ---------------> staging Area(Temporary Area) ------------------> Local Repo ----------------> Remote Repo

Untrackfile = wo files jo git ko pata nhi hoti he - symbol (U).
Staging Area = Wo files jo git add krne k bad staging Area par a jati hn - symbol (A).
Modify = local repo wo changes jo remote repo me modify ya update nhi hue he -  symbol (M).

class-4

Git Ignore
 git ignore hmari project directory mein ek a si file hoti he. jis file k under hum btate he k git  ne kin cheezo ya (Files/directory) ko ignore krna he.in ko track nhi krna he. (.gitignore)

Just Like This:

# Throw the extension agr ksi file ko ignore karna hai to use yaha likho * laga kr
*.css

# kis bhi file ka name k thorw us ko ignore krwya ja skta he 
env

# kisi folder or us k under ki files ko ignore krwya ja skta he
node_modules/

class-5

Git Restore(Like Undo)
working directory me change krne k bad wapis se last commit par wapis ana ho to pehle wala code chaiye ho to us k liye.(working Dir me koi bhi change krne k bad or un changes ko jab tak commit nhi kiya gya he tab tak un ko restore kiya ja skta he)

Track to Untrack: kisi bhi file ya folder ko Track to Untrack krne k liye ye command use krte hn (Before commit tak bs ye command work krti he)
    git restore --staged filename

class-6

Git Revert

working directory  me changes krne k bad un ko commit krne ka bad local ye remote repo mein store krwa diya or us k bad bhi agr xchanges krni ho ya last wala code chaiye ho to waha par phir hum git revert command ka use krte hn. (After Commit to push).

git kiya krta he jab bhi hum commit krte he or agr ek hi commit ek se ziyda bar krte he to git us ki commit ki ek (Hash Value / Hash Code) bana leta he
Hash Value: Basically ek unique value hoti he ap k data ki.(Hash code / Commit code). like jis tarha data bse mein password ki ek unique encrypt value bnate he. bilkul us hi tarha commit ki bhi ek unique encrypted value banti he.or is hi unique value k throw git ko pata chalte he k kab kiya changes hue hn.

in git hash value ya id k throw hum kis bhi last commit ye back to jitne bhi satge jana chae ja skte hn thorw the id code with revert command

git log: git k logs check krne k liye hoti he
git log --oneline: ye latest hash value ko dekhne k liye use hoti he
git revert hash value: jis commit wale part ko undo krna chae kr skte he throw us ki id

