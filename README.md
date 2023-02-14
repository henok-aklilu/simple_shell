<body
<h1> 0x16. C - Simple Shell</h1>

  <div data-react-class="tags/Tags" data-react-props="{&quot;tags&quot;:[{&quot;id&quot;:7,&quot;value&quot;:&quot;C&quot;,&quot;author_id&quot;:null,&quot;created_at&quot;:&quot;2022-06-16T01:59:38.000Z&quot;,&quot;updated_at&quot;:&quot;2022-06-16T01:59:38.000Z&quot;},{&quot;id&quot;:16,&quot;value&quot;:&quot;Group project&quot;,&quot;author_id&quot;:null,&quot;created_at&quot;:&quot;2022-06-16T01:59:38.000Z&quot;,&quot;updated_at&quot;:&quot;2022-06-16T01:59:38.000Z&quot;},{&quot;id&quot;:20,&quot;value&quot;:&quot;Syscall&quot;,&quot;author_id&quot;:null,&quot;created_at&quot;:&quot;2022-06-16T01:59:38.000Z&quot;,&quot;updated_at&quot;:&quot;2022-06-16T01:59:38.000Z&quot;}]}" data-react-cache-id="tags/Tags-0"><div class="align-items-center d-flex flex-wrap gap-3 my-2"><span class="label label-primary" style="font-size: 14px;">C</span><span class="label label-primary" style="font-size: 14px;">Group project</span><span class="label label-primary" style="font-size: 14px;">Syscall</span></div></div>

  <div data-react-class="projects/ProjectMetadata" data-react-props="{&quot;metadata&quot;:{&quot;author&quot;:&quot;Julien Barbier&quot;,&quot;weight&quot;:10,&quot;correction&quot;:{&quot;released&quot;:false,&quot;auto_correction_available_at&quot;:&quot;2023-02-22T01:12:00.000+03:00&quot;,&quot;requires_auto_correction&quot;:true,&quot;requires_manual_correction&quot;:false},&quot;bpi&quot;:{&quot;current&quot;:true,&quot;started&quot;:false,&quot;in_second_deadline&quot;:false,&quot;starts_at&quot;:&quot;2023-02-08T06:00:00.000+03:00&quot;,&quot;ends_at&quot;:&quot;2023-02-23T06:00:00.000+03:00&quot;,&quot;second_deadline_at&quot;:&quot;2023-02-25T06:00:00.000+03:00&quot;},&quot;team&quot;:{&quot;in_team_of&quot;:2,&quot;members&quot;:[&quot;Yoseph Tamirat&quot;,&quot;Henok Aklilu&quot;]}}}" data-react-cache-id="projects/ProjectMetadata-0"><ul class="list-group metadata" id="project-metadata"><li class="list-group-item"><i aria-hidden="true" class="fa fa-user fa-fw"></i> By: Julien Barbier</li><li class="list-group-item"><i aria-hidden="true" class="fa fa-cog fa-fw"></i> Weight: 10</li><li class="list-group-item"><i aria-hidden="true" class="fa fa-users fa-fw"></i> Project to be done in teams of 2 people (your team: Yoseph Tamirat, Henok Aklilu)</li><li class="list-group-item"><i aria-hidden="true" class="fa fa-calendar fa-fw"></i> Project will start <span data-container="body" data-html="false" data-placement="auto top" data-toggle="tooltip" title="" data-original-title="2023-02-08 06:00 (GMT+03:00)"><span class="datetime">Feb 8, 2023 6:00 AM</span></span>, must end by <span data-container="body" data-html="false" data-placement="auto top" data-toggle="tooltip" title="" data-original-title="2023-02-23 06:00 (GMT+03:00)"><span class="datetime">Feb 23, 2023 6:00 AM</span></span></li><li class="list-group-item"><i aria-hidden="true" class="fa fa-check fa-fw"></i> Checker will be released at <span data-container="body" data-html="false" data-placement="auto top" data-toggle="tooltip" title="" data-original-title="2023-02-22 01:12 (GMT+03:00)"><span class="datetime">Feb 22, 2023 1:12 AM</span></span></li><li class="list-group-item"><i aria-hidden="true" class="fa fa-check-square fa-fw"></i> An auto review will be launched at the deadline</li></ul></div>
<div id="project_id" style="display: none" data-project-id="235"></div>  


<h2>Background Context</h2>

<p>Write a simple UNIX command interpreter.</p>

<p><img src="https://s3.amazonaws.com/intranet-projects-files/holbertonschool-low_level_programming/235/shell.jpeg" alt="" loading="lazy" style=""></p>

<p><em>^ “The Gates of Shell”, by <a href="/rltoken/AtYRSM03vJDrko9xHodxFQ" title="Spencer Cheng" target="_blank">Spencer Cheng</a>, featuring <a href="/rltoken/-ezXgcyfhc8qU1DeUInLUA" title="Julien Barbier" target="_blank">Julien Barbier</a></em></p>

<h2>Resources</h2>

<p><strong>Read or watch</strong>:</p>

<ul>
<li><a href="/rltoken/f0YU9TAhniMXWlSXtb64Yw" title="Unix shell" target="_blank">Unix shell</a> </li>
<li><a href="/rltoken/7LJOp2qP7qHUcsOK2-F3qA" title="Thompson shell" target="_blank">Thompson shell</a> </li>
<li><a href="/rltoken/wTSu31ZP1f7fFTJFgRQC7w" title="Ken Thompson" target="_blank">Ken Thompson</a> </li>
<li><strong>Everything you need to know to start coding your own shell</strong> concept page</li>
</ul>

<p><strong>man or help</strong>: </p>

<ul>
<li><code>sh</code> (<em>Run <code>sh</code> as well</em>)</li>
</ul>

<h2>Learning Objectives</h2>

<p>At the end of this project, you are expected to be able to <a href="/rltoken/9LNz86CtOTos9oL3zxIO3A" title="explain to anyone" target="_blank">explain to anyone</a>, <strong>without the help of Google</strong>:</p>

<h3>General</h3>

<ul>
<li>Who designed and implemented the original Unix operating system</li>
<li>Who wrote the first version of the UNIX shell</li>
<li>Who invented the B programming language (the direct predecessor to the C programming language)</li>
<li>Who is Ken Thompson</li>
<li>How does a shell work</li>
<li>What is a pid and a ppid</li>
<li>How to manipulate the environment of the current process</li>
<li>What is the difference between a function and a system call</li>
<li>How to create processes</li>
<li>What are the three prototypes of <code>main</code></li>
<li>How does the shell use the <code>PATH</code> to find the programs</li>
<li>How to execute another program with the <code>execve</code> system call</li>
<li>How to suspend the execution of a process until one of its children terminates</li>
<li>What is <code>EOF</code> / “end-of-file”?</li>
</ul>

<h3>Copyright - Plagiarism</h3>

<ul>
<li>You are tasked to come up with solutions for the tasks below yourself to meet with the above learning objectives.</li>
<li>You will not be able to meet the objectives of this or any following project by copying and pasting someone else’s work. </li>
<li>You are not allowed to publish any content of this project.</li>
<li>Any form of plagiarism is strictly forbidden and will result in removal from the program.</li>
</ul>

<h2>Requirements</h2>

<h3>General</h3>

<ul>
<li>Allowed editors: <code>vi</code>, <code>vim</code>, <code>emacs</code></li>
<li>All your files will be compiled on Ubuntu 20.04 LTS using <code>gcc</code>, using the options <code>-Wall -Werror -Wextra -pedantic -std=gnu89</code></li>
<li>All your files should end with a new line</li>
<li>A <code>README.md</code> file, at the root of the folder of the project is mandatory</li>
<li>Your code should use the <code>Betty</code> style. It will be checked using <a href="https://github.com/holbertonschool/Betty/blob/master/betty-style.pl" title="betty-style.pl" target="_blank">betty-style.pl</a> and <a href="https://github.com/holbertonschool/Betty/blob/master/betty-doc.pl" title="betty-doc.pl" target="_blank">betty-doc.pl</a></li>
<li>Your shell should not have any memory leaks</li>
<li>No more than 5 functions per file</li>
<li>All your header files should be include guarded</li>
<li>Use system calls only when you need to (<a href="/rltoken/EU7B1PTSy14INnZEShpobQ" title="why?" target="_blank">why?</a>)</li>
<li>Write a <code>README</code> with the description of your project</li>
<li>You should have an <code>AUTHORS</code> file at the root of your repository, listing all individuals having contributed content to the repository. Format, see <a href="/rltoken/UL8J3kgl7HBK_Z9iBL3JFg" title="Docker" target="_blank">Docker</a></li>
</ul>

<h3>GitHub</h3>

<p>*<em>There should be one project repository per group. If you and your partner have a repository with the same name in both your accounts, you risk a 0% score. Add your partner as a collaborator. *</em></p>

<h2>More Info</h2>

<h3>Output</h3>

<ul>
<li>Unless specified otherwise, your program <strong>must have the exact same output</strong> as <code>sh</code> (<code>/bin/sh</code>) as well as the exact same error output.</li>
<li>The only difference is when you print an error, the name of the program must be equivalent to your <code>argv[0]</code> (See below)</li>
</ul>

<p>Example of error with <code>sh</code>:</p>

<pre><code>$ echo "qwerty" | /bin/sh
/bin/sh: 1: qwerty: not found
$ echo "qwerty" | /bin/../bin/sh
/bin/../bin/sh: 1: qwerty: not found
$
</code></pre>

<p>Same error with your program <code>hsh</code>:</p>

<pre><code>$ echo "qwerty" | ./hsh
./hsh: 1: qwerty: not found
$ echo "qwerty" | ./././hsh
./././hsh: 1: qwerty: not found
$

</code></pre>

<h3>List of allowed functions and system calls</h3>

<ul>
<li><code>access</code> (man 2 access)</li>
<li><code>chdir</code> (man 2 chdir)</li>
<li><code>close</code> (man 2 close)</li>
<li><code>closedir</code> (man 3 closedir)</li>
<li><code>execve</code> (man 2 execve)</li>
<li><code>exit</code> (man 3 exit)</li>
<li><code>_exit</code> (man 2 _exit)</li>
<li><code>fflush</code> (man 3 fflush)</li>
<li><code>fork</code> (man 2 fork)</li>
<li><code>free</code> (man 3 free)</li>
<li><code>getcwd</code> (man 3 getcwd)</li>
<li><code>getline</code> (man 3 getline)</li>
<li><code>getpid</code> (man 2 getpid)</li>
<li><code>isatty</code> (man 3 isatty)</li>
<li><code>kill</code> (man 2 kill)</li>
<li><code>malloc</code> (man 3 malloc)</li>
<li><code>open</code> (man 2 open)</li>
<li><code>opendir</code> (man 3 opendir)</li>
<li><code>perror</code> (man 3 perror)</li>
<li><code>read</code> (man 2 read)</li>
<li><code>readdir</code> (man 3 readdir)</li>
<li><code>signal</code> (man 2 signal)</li>
<li><code>stat</code> (__xstat) (man 2 stat)</li>
<li><code>lstat</code> (__lxstat) (man 2 lstat)</li>
<li><code>fstat</code> (__fxstat) (man 2 fstat)</li>
<li><code>strtok</code> (man 3 strtok)</li>
<li><code>wait</code> (man 2 wait)</li>
<li><code>waitpid</code> (man 2 waitpid)</li>
<li><code>wait3</code> (man 2 wait3)</li>
<li><code>wait4</code> (man 2 wait4)</li>
<li><code>write</code> (man 2 write)</li>
</ul>

<h3>Compilation</h3>

<p>Your shell will be compiled this way:</p>

<pre><code>gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh
</code></pre>

<h3>Testing</h3>

<p>Your shell should work like this in interactive mode:</p>

<pre><code>$ ./hsh
($) /bin/ls
hsh main.c shell.c
($)
($) exit
$
</code></pre>

<p>But also in non-interactive mode:</p>

<pre><code>$ echo "/bin/ls" | ./hsh
hsh main.c shell.c test_ls_2
$
$ cat test_ls_2
/bin/ls
/bin/ls
$
$ cat test_ls_2 | ./hsh
hsh main.c shell.c test_ls_2
hsh main.c shell.c test_ls_2
$
</code></pre>

<h3>Checks</h3>

<p>The Checker will be released at the end of the project (1-2 days before the deadline). 
We <strong>strongly</strong> encourage the entire class to work together to create a suite of checks covering both regular tests and edge cases for each task. See task <code>8. Test suite</code>.</p>

  </div>
</div>


      

      

        
          <h2 class="gap">Tasks</h2>

    <div data-role="task1033" data-position="1" id="task-num-0">
      <div class="panel panel-default task-card " id="task-1033">
  <span id="user_id" data-id="198536"></span>

  <div class="panel-heading panel-heading-actions">
    <h3 class="panel-title">
      0. Betty would be proud
    </h3>

  
    <h3 class="panel-title">
      1. Simple shell 0.1
    </h3>

    
    <!-- Task Body -->
    <p>Write a UNIX command line interpreter.</p>


<div id="torrent-scanner-popup" style="display: none;"></div></body>
