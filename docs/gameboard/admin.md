# Gameboard Administration

The Admin function of the gameboard app helps those with the admin role:

- Create, clone, manage, and delete games and challenges
- Manage users
- Observe participants
- Enter sponsor information
- Run and export user, gameboard, challenge, and feedback reports
- Broadcast messages to all game participants

After logging into the gameboard app with the appropriate role, click **Admin**.

## Search

This **Search** feature allows game administrators to search on the *name* of the game tiles that appear here.

## Toggle Cards and Table

## Announcement

The **Announcement** feature allows game administrators to broadcast important messages to all participants within a game. Among other uses, these could be messages regarding gameboard issues, challenge issues, and changes to logistics. Announcements appear in the bottom of the gameboard  interface. 

<!--Need to confirm where the announcements appear to the participants.-->

In the Announcement field, enter the content of the announcement and click **Announce**.

## Users

This is where users are assigned roles and participant names are approved or disapproved.

To search for a user across the whole gameboard, enter the term into the **Search** field or filter by:

- **roles:** contains only those participants who have been granted additional roles (Observer, Tester, Designer, etc.)
- **names-pending:** contains only those participants whose display names are pending approval or disapproval from an admin.
- **names-disallowed:** contains only those participants whose display names have been disapproved by an admin.

### Approving and disapproving requested display names

After registering for a new account, players must choose a default name for public display. Players are expected to refrain from any names that are vulgar or political in nature. Admins approve participant names before the names can appear on the scoreboard here. 

To approve a requested display name, click **names-pending**. That gives you a list of players waiting for display name approval. Find the player in the list, select **Approve** or **Disapprove**.

In the screen capture below, Tom Bombadil is requesting a name change to "Treebeard."

![admin-pending](img/admin-pending.png)

If *approved*, the name moves from the **names-pending** list. From the player's point of view, the *requested* display name becomes the display name.

If *disapproved*, you can provide a reason (`disallowed`, `disallowed_pii`, `disallowed_unit`, etc.). The disallowed requested name moves from **names-pending** to **names-disallowed**. From the player's point of view in this instance the *requested* name remains Treebeard, the *approved* name remains Tom Bombadil, and the *display name status* is disallowed. 

## Players

## Sponsors

This is where admins define who the sponsors are and what image to associate with each. **Browse** to or drag a sponsor image into the box. The file name becomes the image "key" and you can now add a title.

In the screen capture below, **moria** is the image key (from the file name) and "Doors of Durin" is the title. There is no save after attaching an image or updating the title.

![moria](img/admin-moria.png)

Click **Delete** then **Confirm** to remove an image and title from the sponsor list.

## Challenges

The Challenges tab is largely for game admins to troubleshoot problems with challenges.

**Search:** Search for specific teams, players,  challenge ids, and tags.

**Current:** *Active* challenges have a green dot next them. Active indicates a challenge has *not* yet been solved correctly, maximum submissions have *not* been attempted, or a session has *not* expired. A challenge is active until one of those three criteria are met; then, the challenge is over and *inactive*. When a challenge is inactive, it still counts towards total score, rank, cumulative time.

A challenge is *current* and not *archived* because it has not been reset when the Reset Session button is clicked. 

**Archived:** When a participant clicks **Reset Session**, before the session is deleted, historical information from participant and challenge event is archived. This archived session information is available here for the game admin to access.

### Audit

Clicking **Audit** provides the game admin with a list of answers submitted by the player.

### Regrade

Clicking **Regrade** has the gameboard check all submissions by a player against expected answers again. Regrade is used when a challenge has two possible answers or players submit in a format that is correct, but that was unexpected by game or challenge developers. When this happens, the TopoMojo workspace is updated manually to include the new correct answers. Then, the challenge is regraded and the player's score updated if a previously entered incorrect answer is now correct.

## Reports

See [Admin Reports](admin-reports.md).