<!DOCTYPE html>
<html>
<body>
	<h1>Mandatory Part</h1>
	<p>Your shell should:</p>
	<ul>
		<li>Display a prompt when waiting for a new command.</li>
		<li>Have a working history.</li>
		<li>Search and launch the right executable (based on the PATH variable or using a relative or an absolute path).</li>
		<li>Not use more than one global variable. Think about it. You will have to explain its purpose.</li>
		<li>Not interpret unclosed quotes or special characters which are not required by the subject such as \ (backslash) or ; (semicolon).</li>
		<li>Handle ' (single quote) which should prevent the shell from interpreting the metacharacters in the quoted sequence.</li>
		<li>Handle " (double quote) which should prevent the shell from interpreting the metacharacters in the quoted sequence except for $ (dollar sign).</li>
		<li>Implement redirections:
			<ul>
				<li>&lt; should redirect input.</li>
				<li>&gt; should redirect output.</li>
				<li>&lt;&lt; should be given a delimiter, then read the input until a line containing the delimiter is seen. However, it doesn’t have to update the history!</li>
				<li>&gt;&gt; should redirect output in append mode.</li>
			</ul>
		</li>
		<li>Implement pipes (| character). The output of each command in the pipeline is connected to the input of the next command via a pipe.</li>
		<li>Handle environment variables ($ followed by a sequence of characters) which should expand to their values.</li>
		<li>Handle $? which should expand to the exit status of the most recently executed foreground pipeline.</li>
		<li>Handle ctrl-C, ctrl-D and ctrl-\ which should behave like in bash.</li>
		<li>In interactive mode:
			<ul>
				<li>ctrl-C displays a new prompt on a new line.</li>
				<li>ctrl-D exits the shell.</li>
				<li>ctrl-\ does nothing.</li>
			</ul>
		</li>
		<li>Your shell must implement the following builtins:
			<ul>
				<li>echo with option -n</li>
				<li>cd with only a relative or absolute path</li>
				<li>pwd with no options</li>
				<li>export with no options</li>
				<li>unset with no options</li>
				<li>env with no options or arguments</li>
				<li>exit with no options</li>
			</ul>
		</li>
		<li>The readline() function can cause memory leaks. You don’t have to fix them. But that doesn’t mean your own code, yes the code you wrote, can have memory leaks.</li>
	</ul>
</body>
</html>
