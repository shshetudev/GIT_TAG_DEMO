<h1>One Min Introduction to GIT TAG!</h1>
<p>In this Tutorial we will learn about Git Tag. It will take just one mintue to get a basic idea about git tag. Let's start<p>
  
  <ul>
  <li><b>What are git tags?</b></li>
  <p>Tagging in git or any other vcs refers to creating specific points in history for your repository/data. This is usually done to mark release points like: v1.0, v1.1, .....</p> <br>
  <li><b>Why should i create git tags?</b></li>
  <p>To mark release points for your code/data. To create historic restore points.</p> <br>
  <li><b>When to create git tags?</b></li>
  <p>When we want to create a release point for a stable version of our code. When we want to create a historic poin for our code/data that can refer at any future time.</p>
  <li><b>How to create tags in Git?</b></li>
  <p>We can create tags in 4 steps:
  <ol>
    <li><b>Checkout to the branch in which we want to attach git tag: </b> git checkout master </li>
    <li>
      <b>Create tag with specific version name: </b> git tag v1.0 <br>
      <b>We can also create annotated tag:</b> git tag -a v1.1 -m "tag for release v1.1" 
    </li>
   <li><b>Display/Show tags: </b> git tag -l "v1.*" </li>
    <li>
      <b>Push tags to remote: </b> git push origin v1.0 <br>
      <b>Push all tags at once: </b> git push origin --tags or git push --tags
    </li>
  </ol>
  </p>
  <li><b>How to delete git tags?</b></li>
  <p>
  <ul>
    <li><b>Delete tag from local: </b> git tag -d v1.0</li>
    <li><b>Delete from remote: </b>
      <ul>
        <li>git push origin -d v1.0</li>
        <li>git push origin --delete v1.0</li>
      </ul>
    </li>
    <li><b>Delete multiple tags at once:</b> 
      <ul>
        <b>Delete from local: </b> git tag -d v1.0 v1.1 <br>
        <b>Delete from remote: </b> git push origin -d v1.0 v1.1
      </ul>
    </li>
</ul>
</p> <br>
  <li><b>How do we checkout tags in git?</b></li>
  <p>
  We can't checkout tags in Git. We can create a branch from a tag and checkout the branch: git checkout -b releasevar1 v1.0
  </p> <br>
  <li><b>Can i create a tag from some past commit?</b></li>
  <p>
  Yes. git tag v1.2 5fcdb03(commit name)
  </p>
</ul>
