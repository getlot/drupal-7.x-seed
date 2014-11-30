Drupal 7.x seed

init

git remote add drupal git://git.drupal.org/project/drupal.git

update drupal

git fetch drupal  # Get all the latest from drupal.org
git merge 7.x    # Merge the latest Drupal from the drupal.org 7.x branch
git push origin seed   # push these new changes to our remote


add submodule

dev:
add submodule
git submodule add git://git.drupal.org/project/examples.git sites/all/modules/examples
cd sites/all/modules/examples
git checkout tag
cd ..
git add sites/all/modules/examples
git commit -m "moved submodule to v1.0"
git push

update submodule with a tag

dev:
cd sites/all/modules/examples
git fetch
git checkout tag
cd ..
git push

prod:
git pull
git submodule update --init
drush updatedb
drush cc all


remove submodule
git submodule deinit asubmodule
git rm asubmodule
rm -rf .git/modules/asubmodule
