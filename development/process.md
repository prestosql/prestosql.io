---
layout: page
menu_id: development
title: Development - Process
---

<div class="leftcol widecol process">
    <h2>Contribution Process</h2>

    <p>
    This is the process we suggest for contributions.  This process is designed to reduce the burden on project reviews, impact on other contributors, and to keep the amount of rework from the contributor to a minimum.
    </p>

    <p>
    <ol>
    <li>Sign the <a href="https://github.com/prestosql/cla">contributor license agreement</a>.</li>
    <li>Start a discussion by creating a Github <a href="https://github.com/prestosql/presto/issues">issue</a>, or asking on
        <a href="https://join.slack.com/t/prestodb/shared_invite/enQtNDczNzEzMjYxMTc0LTc5MTVmZjE1N2E4YjJmZDBlNDBkOGUwMjM5YWIwM2E1ZjI3M2FiYzk2MTRmZjFjYjQ3ZmIwNzAzZTU5MWM4ZGU">Slack</a>
        (unless the change is trivial).
        <ol>
            <li>This step will help you identify possible collaborators and reviewers.</li>
            <li>Does the change align with technical vision and project values?</li>
            <li>Will the change conflict with another change in progress? If so, work with others to minimize impact.</li>
            <li>Is this change large?  If so, work with others to break into smaller steps.</li>
        </ol>
    </li>
    <li>Implement the change
        <ol>
            <li>If the change is large, post a preview Github <a href="https://github.com/prestosql/presto/pulls">pull request</a> with the title prefixed with <code>[WIP]</code>, and share with collaborators.</li>
            <li>Include tests and documentation as necessary.</li>
        </ol>
    </li>
    <li>Create a Github <a href="https://github.com/prestosql/presto/pulls">pull request</a> (PR).
        <ol>
            <li>Make sure the pull request passes the tests in Travis CI.</li>
            <li>If known, request a review from an expert in the area changed.  If unknown, ask for help on Slack.</li>
        </ol>
    </li>
    <li>Review will be performed by one or more reviewers.
        <ol>
            <li>This normally happens within a few days, but may take longer if the change is large, complex, or if a critical reviewer is unavailable. (feel free to ping the pull request)</li>
        </ol>
    </li>
    <li>Address concerns and update the pull request.
        <ol>
            <li>Comments will be attached to each individual commit in the pull, and changes should be addressed in a new <code>Fixup!</code> commit placed after each commit.  This is to make it easier for the reviewer to see the what was updated.</li>
            <li>After pushing the changes, add a comment to the pull-request, mentioning the reviewers by name, stating the change have been addressed.  This is the only way that a reviewer is notified that you are ready for the code to be reviewed again.</li>
            <li>Go to step 5.</li>
        </ol>
    </li>
    <li>Committer will merge the pull request after final changes are accepted.</li>
    <li>Add release notes to the <a href="https://github.com/prestosql/presto/labels/release-notes">issue</a> for the upcoming release.</li>
    </ol>
    </p>
</div>
