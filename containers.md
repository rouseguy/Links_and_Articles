MiniShift

Download: VirtualBox
Install mini shift using brew
Install Compose using brew
docker-compose -f docker-compose-katappa.yml build
kompose -f docker-compose-katappa.yml convert -o kattappa_ms.json --provider=openshift

brew tap caskroom/versions
brew cask install minishift-beta

minishift start --vm-driver="virtualbox"

export PATH=$PATH:~/.minishift/cache/oc/v1.5.0-rc.0

oc secrets new-basicauth kattappasecret --username=USERNAME --password=PASSWORD
oc secrets new-basicauth kattappasecret --username=USERNAME --password=PASSWORD --gitconfig=.gitconfig

oc secrets add serviceaccount/builder secrets/kattappasecret


minishift console


Error came. So, commented out build from the yml file



oc login
minishift docker-env
eval $(mini shift docker-env)
docker-compose -f docker-compose-kattappa.yml build
(Need to deployment yaml)
oc create -f .



docker images   (to check if docker image got created)

(Removed manifest normaliser from the yml files)




Install powershift

Install OC
Add it to path
 export PATH=~/.powershift/tools:$PATH

oc login cluster-name
oc new-project project-name
oc secrets new-basicauth kattappasecret --username=USERNAME --password=PASSWORD
oc secrets add serviceaccount/builder secrets/kattappasecret
oc secrets add serviceaccount/builder secret/kattappasecret




Start MiniShift
Oc login to the ip
Oc new-project kattappa
Move into oc_config folder
Oc delete project kattappa

Minishift docker-env
Eval $(minishift docker-env)
Go back to cd ..
docker-compose -f docker-compose-katappa.yml build
Oc new-project kattappa
cd oc_config
Oc create -f .

