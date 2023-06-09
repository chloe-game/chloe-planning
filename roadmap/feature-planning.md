# Feature Planning

For now, these items will be listed here. Eventually they will be moved to a
project board for tracking.

## Must Haves

### Optimization

- Performance Optimization

  - **Priority:** Critical
  - **Complexity:** High
  - **User Story:** As a player, I do not need specialized gaming hardware to
    enjoy this experience.
  - Performance tuning will be a major focus of this effort. The game must be
    able to run on a "standard developer laptop".

    Using the below laptop as an example:

    - OS: Windows 10/macOS Catalina
    - CPU: Intel i5, AMD Ryzen 5
    - RAM: 16GB
    - Storage: 256GB (SSD)
    - Resolution: 1920x1080

### Game World

- Evolving Background
  - **Priority:** Low
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to see the game world change in
    response to my progress through the main story.
  - Each level is its own contained scene; it is not an open-world game. As the
    player completes levels, the environment changes to reflect new resources
    and workloads being deployed into the company's AWS account. These would not
    be interactable, but would be animated to show changing/scaling workloads.
- Characters
  - **Priority:** Critical
  - **Complexity:** High
  - **User Story:** As a player, I can interact with CHLOE and boss characters
    in the game.
  - CHLOE and bosses will be the only NPCs physically represented in-game. Each
    will end up having unique animations for different purposes, with CHLOE's
    being more complex.
- World
  - **Priority:** Medium
  - **Complexity:** Low
  - **User Story:** As a player, my game world is represented as an AWS account.
  - An "empty" AWS account is initially a (seemingly) infinite open plane.
- Graphics - AWS Resources
  - **Priority:** Medium
  - **Complexity:** Low
  - **User Story:** As a player, I can see different representations of AWS
    resources in the game world.
  - Each resource type that the game supports will need to have it's own mesh.
    The meshes themselves will likely require different LOD/complexity to
    support low-end graphics.
- Player Character
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can customize my appearance in the game
    world.
  - The player will have a customizable avatar to represent them. Though they
    would not see this in first-person gameplay, it will be visible in future
    multiplayer as well as shareable on social media.
- Physics
  - **Priority:** Low
  - **Complexity:** Low
  - **User Story:** As a player, I am not bound by physics in the game world.
  - The player and their navigation are not bound by physics. Neither are bosses
    or CHLOE.

### Audio

- Music

  - **Priority:** High
  - **Complexity:** High
  - **User Story:** As a player, I am able to listen to music while playing the
    game.
  - We would initially outsource creation of some number of songs for background
    music, or purchase existing audio with an appropriate license.

    Songs:

    - Main Menu
    - Simulation Mode (rotate through some # of songs)
    - Game Levels (need to determine number of levels)

    Stretch: Customizing the music based on the mood/story within the level.

- Player - Footsteps
  - **Priority:** Low
  - **Complexity:** Low
  - **User Story:** As a player, I can hear my footsteps when walking on ground.
  - Footstep sound plays when not flying.
- Player - Open/Close Menu
  - **Priority:** Medium
  - **Complexity:** Low
  - **User Story:** As a player, I can hear the sound of opening and closing the
    menus.
  - Opening/closing the menu would play an animation of the menu hologram
    originating from the player's hand. The sound effect would be played during
    the open/close animation.
- Menu - Navigation
  - **Priority:** Low
  - **Complexity:** Low
  - **User Story:** As a player, I can hear when I switch between menu options.
  - Applies to all menus (main, pause, etc.).
- Menu - Select
  - **Priority:** Low
  - **Complexity:** Low
  - **User Story:** As a player, I can hear when I select a menu option.
  - Confirmation sound. Applies to all menus.
- CHLOE - "Chitter"
  - **Priority:** Low
  - **Complexity:** Low
  - **User Story:** As a player, I can hear when CHLOE is speaking.
  - CHLOE dialog is not actually voiced, but some kind of "chitter" sound would
    help give the player the feeling that she is speaking while the dialog
    prints on screen.
- CHLOE - Resource Launch
  - **Priority:** Medium
  - **Complexity:** Low
  - **User Story:** As a player, I can hear when CHLOE launches an AWS resource.
- CHLOE - Resource Update
  - **Priority:** Medium
  - **Complexity:** Low
  - **User Story:** As a player, I can hear when CHLOE updates an AWS resource.
  - Should be different than a launch to help the player distinguish.
- CHLOE - Resource Terminate
  - **Priority:** Medium
  - **Complexity:** Low
  - **User Story:** As a player, I can hear when CHLOE terminates an AWS
    resource.
- CHLOE - Attention
  - **Priority:** Low
  - **Complexity:** Low
  - **User Story:** As a player, I can hear when CHLOE is paying attention after
    I call her.
  - Something akin to a "Hmm?"
- Interaction - What is this for?
  - **Priority:** Medium
  - **Complexity:** Low
  - **User Story:** As a player, I can hear when CHLOE is performing an
    architecture demonstration.
  - Would be a series of combined sounds as part of the animation. Could
    potentially be made up of a combination of other "core" sounds.
- Interaction - How do I?
  - **Priority:** Medium
  - **Complexity:** Low
  - **User Story:** As a player, I can hear when CHLOE is performing an
    architecture demonstration.
  - Would be a series of combined sounds as part of the animation. Could
    potentially be made up of a combination of other "core" sounds.
- Interaction - How do I? - Create
  - **Priority:** Medium
  - **Complexity:** Low
  - **User Story:** As a player, I can hear when I ask CHLOE to create the
    resources that make up a "How do I?" demonstration.
  - This sound would occur to denote that the mock resources are not being
    cleaned up, and the player is free to modify and launch them.
- Interaction - How do I? - Destroy
  - **Priority:** Medium
  - **Complexity:** Low
  - **User Story:** As a player, I can hear when I ask CHLOE to destroy the
    resources that make up a "How do I?" demonstration.
  - This sound would occur to denote that the mock resources are being cleaned
    up.
- AWS Resource - Notification
  - **Priority:** Medium
  - **Complexity:** Low
  - **User Story:** As a player, I can hear when there is something wrong with
    an AWS resource I am in range of.
  - Launch, Update, Terminate failures.
- Boss - "Chitter"
  - **Priority:** Low
  - **Complexity:** Low
  - **User Story:** As a player, I can hear when a boss is speaking.
  - Would be unique pitch/timber/etc. for different bosses. I.E. Chaos Monkey
    would be lower and slower than Bees with Machine Guns.
- Boss - Attack
  - **Priority:** Low
  - **Complexity:** Low
  - **User Story:** As a player, I can hear when a boss is attacking AWS
    resources.
  - Would be unique for each boss.
- Boss - Harmed
  - **Priority:** Low
  - **Complexity:** Low
  - **User Story:** As a player, I can hear when a boss is harmed.
  - Would be unique for each boss.
- Boss - Won
  - **Priority:** Low
  - **Complexity:** Low
  - **User Story:** As a player, I can hear when a boss defeats me.
  - Would be unique for each boss.
- Boss - Lost
  - **Priority:** Low
  - **Complexity:** Low
  - **User Story:** As a player, I can hear when I defeat a boss.
  - Would be unique for each boss.

## Game Levels

- Core Levels
  - **Priority:** Critical
  - **Complexity:** High
  - **User Story:** As a player, I have access to a number of levels that follow
    a coherent story.
  - Requires further breakdown into individual levels and their components.
    Would cover the five Well-Architected Pillars. Outline what levels are used
    for onboarding/tutorials and how that is scaffolded across the story.
- Bosses

  - **Priority:** Critical
  - **Complexity:** High
  - **User Story:** As a player, I am able to fight against bosses in certain
    Game Mode levels.
  - Boss battles take place at the end of each Well-Architected questline, as
    well as at the end of the main story. Boss battles are timed events (the
    boss is actively destroying the environment around the player, and will
    complete this task as some point).

    TBD - Need to do high level story write up and determine the initial set of
    bosses.

- Narrative
  - **Priority:** Critical
  - **Complexity:** Medium
  - **User Story:** As a player, I am driven to complete the game by a narrative
    that makes my role important.
  - TBD - Need to do high level story write up.
- Dialog

  - **Priority:** Critical
  - **Complexity:** Medium
  - **User Story:** As a player, I can perform some dialog with NPCs.
  - The dialog itself is scripted.

    TBD - Need to do high level story write up. Have to determine what branches
    would exist in the story that are affected by player choice (if any).

- Player Mail
  - **Priority:** Medium
  - **Complexity:** Low
  - **User Story:** As a player, I sometimes receive mail from my company.
  - Mail is used to provide additional story context, as well as side missions
    during levels.
- Side Missions

  - **Priority:** Low
  - **Complexity:** Medium
  - **User Story:** As a player, I sometimes receive side missions from my
    company.
  - Missions themselves would be short learning experiences around a particular
    use case (i.e. a person needs a password reset).

    TBD - Write up some example missions. Would need to have entire list written
    with Curriculum Developers.

## Updates

- Content Updates
  - **Priority:** High
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to receive content updates
    automatically whenever I start the game.
  - Content updates are defined as changes and additions to the game experience,
    such as new levels. The updates themselves do not need to be ready on
    initial release, but the functionality must exist. Need to investigate the
    complexity of doing with a standalone launcher and/or Steam and similar
    clients.
- Functionalty Updates
  - **Priority:** High
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to receive functionality updates
    automatically whenever I start the game.
  - Functionality updates are defined as changes to the gameplay mechanics and
    loops, such as support for new AWS services. The updates themselves do not
    need to be ready on initial release, but the functionality must exist. Need
    to investigate the complexity of doing with a standalone launcher and/or
    Steam and similar clients."
- Patch Notes
  - **Priority:** Low
  - **Complexity:** Low
  - **User Story:** As a player, I am able to view historical patch notes for
    the game.
  - This can be hosted in the game launcher itself, or on a static website.

## Authentication and Profile Storage

- Steam Integration
  - **Priority:** Medium
  - **Complexity:** Medium
  - **User Story:** As a player, my progress, achievements, badges, and other
    metadata are stored within my Steam profile (if I am running the game using
    the Steam client).
  - Logging in will allow the game to store player save data, learner history,
    etc. Includes progress, learning history, achievements, and other player
    metadata as needed. Information is encrypted at rest and in transit.
- Local Storage
  - **Priority:** Medium
  - **Complexity:** Medium
  - **User Story:** As a player, my progress, achievements, badges, and other
    metadata are stored locally on my computer.
  - Would need to be able to reconcile this with cloud saves and prompt the user
    if one is more "fresh" than the other.

## Player Profile

- Personal Profile
  - **Priority:** Medium
  - **Complexity:** Medium
  - **User Story:** As a player, I can create a personal game profile that
    persists across multiple gameplay sessions.
  - Includes save data, player progression, achievements, badges, etc.
- Avatar
  - **Priority:** Low
  - **Complexity:** Medium
  - **User Story:** As a player, I can create and customize an avatar that
    represents me.
  - Would be visible in game world (for multiplayer support).
- Avatar - Sharing
  - **Priority:** Low
  - **Complexity:** Medium
  - **User Story:** As a player, I can share my avatar to social media.
  - This can be shared as an image to social media.
- Avatar - Customizations
  - **Priority:** Low
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to unlock and apply customizations to
    my player avatar after completing certain badges or achievements.
  - These can be considered unlockable content that the player can use to
    customize their avatar. Examples include hairstyles, swag, and clothes.
- Settings
  - **Priority:** High
  - **Complexity:** Low
  - **User Story:** As a player, my prefered settings are saved automatically.
  - This is saved in the player preferences.
- Badges
  - **Priority:** Medium
  - **Complexity:** Medium
  - **User Story:** As a player, I will receive virtual badges when completing
    specific learning goals.
  - Badges track learning progress and goals. Badge data would sync Steam, Epic,
    etc. Specific Badges TBD.
- Achievements
  - **Priority:** Medium
  - **Complexity:** Medium
  - **User Story:** As a player, I will receive achievements when completing
    specific tasks.
  - Achievements track different individual tasks, not specific learning goals.
    More for fun/collection.
- Personal Data Removal
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I have the option to request deletion of all my
    data related to this game.
  - Needed to support GDPR compliance, but need to determine if this would be
    relevant based on the goal of not storing **any** personal data.

## Main Menu

- Main Menu
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, the first thing I see when I launch the game is
    the main menu.
  - The UI for the launch screen of the main menu can be straightforward, but
    art/sound assets may require more development.
- Main Menu - Select Level
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can select an option in the main menu to view
    the list of available levels.
  - The player would be able to see any levels they have already completed, as
    well as the next incomplete level (if any).
- Main Menu - Simulation Mode
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can select an option in the main menu to open
    Simulation Mode.
  - When opening Simulation Mode, the player is initially prompted to select the
    AWS profile they wish to use, or disable live AWS integration. If the player
    used Simulation Mode previously, the past setting will be the default.
- Avatar Creator
  - **Priority:** Medium
  - **Complexity:** Low
  - **User Story:** As a player, I can select an option in the main menu to
    create and/or update my avatar.
  - The player would have access to an initial set of customizations (hair, skin
    tone, body shape, clothes, etc.), with more unlocked either through
    gameplay, achievements, or unlockable codes.
- Main Menu - Exit to Desktop
  - **Priority:** Critical
  - **Complexity:** Medium
  - **User Story:** As a player, I can select an option in the main menu to exit
    the application and return to the desktop.
  - Player progress and settings should be saved automatically.
- Main Menu - Settings
  - **Priority:** Critical
  - **Complexity:** Medium
  - **User Story:** As a player, I can adjust preferences such as controls,
    graphics quality, sound levels, and more.
  - Not an exhaustive list, but players should be able to change:
    - Volume: Master, FX, Music, Audio Playback
    - Graphics (Presets): Low, Medium, High, Ultra
    - Graphics: Fullscreen/Windowed/Borderless, Brightness, Contrast, Gamma,
      Resolution, Texture Quality, Particle Effect Quality, Depth of Field,
      Anti-Aliasing, Shadow Quality, Anti-Aliasing, FOV, Color Blind Mode
    - Controls (Mouse/Keyboard): Mouse Sensitivity, Invert Axis, Key Bindings
    - Game: AWS Profile, Resource Synchronization Rate
- Main Menu - Feedback
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can submit anonymous feedback from the main
    menu.
  - This needs to be stored in a data warehouse, details TBD.

## Level Select

- Level List
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, choosing the Select Level option in the main
    menu will present me with a list of available levels to play.
  - The level list should include:
    - Level Number
    - Level Name
    - Description
    - Focus (AWS Well Architected Pillar, Intro, etc.)
    - AWS Services Covered
- Level Launch
  - **Priority:** Critical
  - **Complexity:** Medium
  - **User Story:** As a player, I can choose an available level from the list
    to launch.
  - When launching an already completed level, the player must restart the level
    from the beginning. When launching an incomplete level, the player can
    choose to continue from where they left off, or restart from the beginning.

## Player Control

- Mouse/Keyboard Controls - Player
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can control my "avatar" using a keyboard and
    mouse.
  - This implementation is fairly standard and can be pulled from existing
    examples. Players can run, strafe, look, fly, and interact.
- Mouse/Keyboard Controls - Menus
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can navigate menus using a keyboard and
    mouse.
  - In menus, the cursor is visible and menu controls are clickable.
    Alternatively, keyboard controls (arrow keys, enter, escape, etc.) can be
    used to navigate the menu flow.

## Game Mechanics

- Replayability
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can replay any Game Mode level I completed
    previously.
  - Players may wish to review a previous learning.
- AWS Profile - Disabled
  - **Priority:** Low
  - **Complexity:** Low
  - **User Story:** As a player, I am **not** able to enable AWS integration
    while playing Game Mode.
  - The game levels would be more about general education, with less focus on
    creating live resources. Additionally, we do not want customers to have to
    pay for running resources while playing a game.
- Evolving Backgound
  - **Priority:** Low
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to see the game world change in
    response to my progress through the main story.
  - Each level is its own contained scene; it is not an open-world game. As the
    player completes levels, the environment changes to reflect new resources
    and workloads being deployed into the company's AWS account. These would not
    be interactable, but would be animated to show changing/scaling workloads.
- Menu - Exit to Main Menu
  - **Priority:** Low
  - **Complexity:** Low
  - **User Story:** As a player, I can select an option in the game menu to exit
    the current level/mode and return to the main menu.
  - Player settings should be saved automatically.
- Menu - Settings
  - **Priority:** Critical
  - **Complexity:** Medium
  - **User Story:** As a player, I can adjust preferences such as controls,
    graphics quality, sound levels, and more.
  - Not an exhaustive list, but players should be able to change:
    - Volume: Master, FX, Music
    - Graphics (Presets): Low, Medium, High, Ultra
    - Graphics: Fullscreen/Windowed/Borderless, Brightness, Contrast, Gamma,
      Resolution, Texture Quality, Particle Effect Quality, Depth of Field,
      Anti-Aliasing, Shadow Quality, Anti-Aliasing, FOV, Color Blind Mode
    - Controls (Mouse/Keyboard): Mouse Sensitivity, Invert Axis, Key Bindings
    - Game: AWS Profile, Resource Synchronization Rate"
- Menu - Feedback
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can submit anonymous feedback from the game
    menu.
  - This needs to be stored in a data warehouse.
- AWS Resource Selection
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can open a menu to select the AWS resource I
    want to create.
  - Players can filter by specific AWS services, and can see preview information
    about the service and resource (text, instructional videos, use cases,
    etc.). Implemented in camera space.
- AWS Resource Configuration
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can open a menu to modify the configuration
    of an AWS resource I am creating.
  - Resource properties are rendered in this menu based on the type (i.e.
    boolean, select from list, editable list, text, etc.). Implemented in world
    space from the resource in question.
- Resource Positioning
  - **Priority:** Critical
  - **Complexity:** High
  - **User Story:** As a player, when I enable resource synchronization, AWS
    resources in my game world are synced from my AWS account and are organized
    in a logical manner.
  - Need to define organization/presentation rules...this will likely be very
    complex. Container resources can be nested within one another. Nested
    resources (container and individual) cannot be positoned outside their
    parent resource.

## Simulation Mode

- Simulation Mode
  - **Priority:** Critical
  - **Complexity:** High
  - **User Story:** As a player, I can connect my own AWS account(s) and
    visualize/manage them within the application.
  - The game itself will introduce the core functionality needed to make this
    happen, but the amount of work needed for ongoing service/feature support
    will be very high.
- Menu - Initial Launch
  - **Priority:** Low
  - **Complexity:** Low
  - **User Story:** As a player, I am prompted to set an AWS profile when
    launching Simulation Mode.
  - Initially this will be set to the previous value (if the player used
    Simlation Mode in the past). The player can choose the preselected profile,
    select another, or disable the integration.
- AWS Profile - Single Account
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can choose one of the AWS CLI profiles
    configured on my computer to connect to the game.
  - Already in POC. Game needs to read the AWS CLI credential files and provide
    the list back to the user.
- AWS Profile - Disabled
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can choose to disable AWS integration with
    the game.
  - Already in POC. If the client is disabled, all CRUD requests for AWS
    resources are simply not sent to the AWS endpoints.
- Menu - Exit to Main Menu
  - **Priority:** Low
  - **Complexity:** Low
  - **User Story:** As a player, I can select an option in the game menu to exit
    the current level/mode and return to the main menu.
  - Player settings should be saved automatically.
- Menu - Settings
  - **Priority:** Critical
  - **Complexity:** Medium
  - **User Story:** As a player, I can adjust preferences such as controls,
    graphics quality, sound levels, and more.
  - Not an exhaustive list, but players should be able to change:
    - Volume: Master, FX, Music
    - Graphics (Presets): Low, Medium, High, Ultra
    - Graphics: Fullscreen/Windowed/Borderless, Brightness, Contrast, Gamma,
      Resolution, Texture Quality, Particle Effect Quality, Depth of Field,
      Anti-Aliasing, Shadow Quality, Anti-Aliasing, FOV, Color Blind Mode
    - Controls (Mouse/Keyboard): Mouse Sensitivity, Invert Axis, Key Bindings
    - Game: AWS Profile, Resource Synchronization Rate"
- Menu - Feedback
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can submit anonymous feedback from the game
    menu.
  - This needs to be stored in a data warehouse.
- AWS Resource Selection
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can open a menu to select the AWS resource I
    want to create.
  - Players can filter by specific AWS services, and can see preview information
    about the service and resource (text, instructional videos, use cases,
    etc.). Implemented in camera space.
- AWS Resource Configuration
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can open a menu to modify the configuration
    of an AWS resource I am creating.
  - Resource properties are rendered in this menu based on the type (i.e.
    boolean, select from list, editable list, text, etc.). Implemented in world
    space from the resource in question.
- Resource Positioning
  - **Priority:** Critical
  - **Complexity:** High
  - **User Story:** As a player, when I enable resource synchronization, AWS
    resources in my game world are synced from my AWS account and are organized
    in a logical manner.
  - Need to define organization/presentation rules...this will likely be very
    complex. Container resources can be nested within one another. Nested
    resources (container and individual) cannot be positoned outside their
    parent resource.

## AWS

- Individual Resources
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I am able to see resources that do not contain
    other resources.
  - Individual resources:
    - Have a unique ID.
    - Do not contain other resources.
    - May reference other resources.
    - May be contained by other resources.
    - Example: EC2 Instance
- Container Resources
  - **Priority:** Critical
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to see resources that act as
    containers of other resources.
  - Container resources:
    - Have a unique ID.
    - May contain other resources (individual and container).
    - May reference other resources.
    - May be contained by other resources.
    - Example: VPC
- Property-Based Resources
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I am able to see individual, property based
    resources.
  - Property based resources:
    - Do not have a unique ID (they are defined by their property values, and
      must be tracked accordingly).
    - Do not contain other resources.
    - May reference other resources.
    - May be contained by other resources.
    - Example: Network ACL Entry

## Core AWS Service Support

List is not definitive yet. Will depend on the story/level outline.

- Amazon S3 Support
  - **Priority:** Critical
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to create, read, update, and delete
    (CRUD) Amazon S3 resources.
  - Resources:
    - Bucket
    - BucketPolicy
  - Example Transformations:
    - Different storage classes will use different "variants" of the same S3
      bucket mesh.
    - Buckets with public access enabled will have different color/highlighting.
- AWS IAM Support
  - **Priority:** Critical
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to create, read, update, and delete
    (CRUD) IAM resources.
  - Resources:
    - Group
    - InstanceProfile
    - ManagedPolicy
    - Policy
    - Role
    - User
    - UserToGroupAddition
  - Example Transformations:
    - Roles, Users, and Policies with administrator/power user access will have
      different color/highlighting.
    - Roles and Users with many policies will be larger than Roles and Users
      with fewer policies (managed and/or inline).
    - UserToGroupAddition is represented as a property-based resource (link).
- Amazon VPC Support
  - **Priority:** Critical
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to create, read, update, and delete
    (CRUD) Amazon VPC resources.
  - Resources:
    - InternetGateway
    - NatGateway
    - NetworkAcl
    - NetworkAclEntry
    - Route
    - RouteTable
    - SecurityGroup
    - SecurityGroupEgress
    - SecurityGroupIngress
    - Subnet
    - SubnetCidrBlock
    - SubnetNetworkAclAssociation (Property-based resource link)
    - SubnetRouteTableAssociation (Property-based resource link)
    - VPC
    - VPCCidrBlock
  - Example Transformations:
    - VPC, Subnet, Security Group transform scales to contain all nested
      resources.
    - Route table highlighting for internet-accessible routes.
    - Security group highlighting for SSH from anywhere ingress rules."
- Amazon EC2 Support
  - **Priority:** Critical
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to create, read, update, and delete
    (CRUD) Amazon EC2 resources.
  - Resources:
    - EIP
    - EIPAssociation (Property-based resource link)
    - Instance
    - LaunchTemplate
    - NetworkInterface
    - NetworkInterfaceAttachment (Property-based resource link)
    - NetworkInterfacePermission
    - Volume
    - VolumeAttachment
  - Example Transformations:
    - Instance type is represented as text on the resource's mesh.
- AWS Auto Scaling Support
  - **Priority:** Critical
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to create, read, update, and delete
    (CRUD) AWS Auto Scaling resources.
  - Resources:
    - ScalingPlan
  - Example Transformations:
    - Animations when the scaling plan kicks in to add more instances to the
      group.
- AWS Lambda Support
  - **Priority:** Critical
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to create, read, update, and delete
    (CRUD) AWS Lambda resources.
  - Resources:
    - Alias
    - EventSourceMapping
    - Function
    - Permission
    - Version
  - Example Transformations:
    - TBD
- Amazon DynamoDB Support
  - **Priority:** Critical
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to create, read, update, and delete
    (CRUD) Amazon DynamoDB resources.
  - Resources:
    - GlobalTable
    - Table
  - Example Transformations:
    - Transform size change based on R/W capacity units.
- Amazon RDS Support
  - **Priority:** Critical
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to create, read, update, and delete
    (CRUD) Amazon RDS resources.
  - Resources:
    - DBInstance
    - DBParameterGroup
    - DBSecurityGroup
    - DBSecurityGroupIngress
    - DBSubnetGroup
- Example Transformations:
  - DB instance type is represented as text on the resource's mesh.
- Amazon SNS Support
  - **Priority:** Critical
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to create, read, update, and delete
    (CRUD) Amazon SNS resources.
  - Resources:
    - Subscription (Property-based resource link)
    - Topic
    - TopicPolicy
  - Example Transformations:
    - Subscription represented as a link between the Topic and the subscriber
      (if it is an AWS resource in the same account).
- Amazon SQS Support
  - **Priority:** Critical
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to create, read, update, and delete
    (CRUD) Amazon SQS resources.
  - Resources:
    - Queue
    - QueuePolicy
  - Example Transformations:
    - Queue transform scale based on number of messages present.
- Amazon CloudWatch Support
  - **Priority:** Critical
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to create, read, update, and delete
    (CRUD) Amazon CloudWatch resources.
  - Resources:
    - Alarm
  - Example Transformations:
    - Color, scale, animation when Alarm is raised.
- Amazon Route53 Support
  - **Priority:** Critical
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to create, read, update, and delete
    (CRUD) Amazon Route53 resources.
  - Resources:
    - HostedZone
    - RecordSet
    - RecordSetGroup
  - Example Transformations:
    - TBD
- Resource Sync - Single Account
  - **Priority:** Critical
  - **Complexity:** Very High
  - **User Story:** As a player, my game client automatically syncs with my
    linked AWS account to pull the current state of supported resources.
  - TBD: Will this require launching resources in the customer account? **It is
    critical that this be fast. It is not useful to have to wait 5-10 minutes
    for this to sync.**"
- Resource Linking
  - **Priority:** Critical
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to see when resources are linked
    and/or depend on one another.
  - This should not presented for every resource all the time. TBD - Need to
    test different approaches to how this presents.
    - If the distance is below a certain threshold, show as a line from origin
      resource to related resource.
    - If the distance is above a certain threshold, create a "portal" to
      teleport to the related resource (and back).
  - Parent to child:
    - The player can view a resource, and then view related resources based on
      the property values. When selecting a property value that includes a
      related resource, there is an option to ""locate"" that resource.
  - Child to parent:
    - The player can select a control to get a list of resources that reference
      the currently selected resource.
- Manual Resource Linking
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can create logical links between resources.
  - Unlike relationship links based on resource properties, these would be
    presented all the time (until one of the linked resources is terminated).
    Players will use this to create their own architecture diagrams.
- Resource Errors
  - **Priority:** Medium
  - **Complexity:** Low
  - **User Story:** As a player, I can see details when a resource fails to
    launch, update, or terminate.
  - Players need to see the API error results when AWS actions fail.
    - An animation loops on the resource to show it is in an error state.
    - An alarm sound loops when the player is in proximity (this can be
      disabled).
- Offline Property Validation
  - **Priority:** High
  - **Complexity:** High
  - **User Story:** As a player, I receive validation errors for incorrect
    resource properties, even when playing the game offline (or without AWS
    integration enabled).
  - This is helpful for learning so players can see more info on what they did
    wrong. Also serves as a helpful point to avoid unnecessary AWS API calls.
- Resource Movement
  - **Priority:** Low
  - **Complexity:** Low
  - **User Story:** As a player, I can "grab" launched resources in the
    environment and move them to a location of my choosing.
  - Players want to create their own living architecture diagrams. This impacted
    by the type of resource and what can/can't be moved. Container resources can
    be moved only within their respective container (if they are in one).
    Individual resources can only be moved if they are not in a container.

## Training

- JIT Training - Audio Explanations
  - **Priority:** High
  - **Complexity:** Low
  - **User Story:** As a player, I can get audio explanations of AWS services,
    resources, and resource properties.
  - When working with a service, resource, or property, a control will exist for
    the player to prompt the game to play an audio clip giving more information
    on the specific element. A speaker icon next to the element.
- JIT Training - Video Tutorials
  - **Priority:** Medium
  - **Complexity:** Low
  - **User Story:** As a player, I can get video explanations of AWS services,
    resources, and resource properties.
  - When working with a service, resource, or property, a control will exist for
    the player to prompt the game to play a video clip giving more information
    on the specific element. A video icon next to the element. The video
    playback will anchor on the HUD in camera space.
- JIT Training - In-Game Architecture Demonstrations
  - **Priority:** Low
  - **Complexity:** High
  - **User Story:** As a player, I can get architecture demonstrations of AWS
    services and resources.
  - When working with a service or resource (not a resource property), a control
    will exist for the player to prompt the game to play an architecture
    demonstration on the specific element.
    - A demo icon next to the element.
    - CHLOE will perform the architecture demo in world space.
    - An audio explanation will play.
    - A text explanation will appear in the HUD in camera space.
    - Alternate option: Have the CHLOE demo play in the HUD as video."

## Socialization

- Twitch Streams
  - **Priority:** Low
  - **Complexity:** Low
  - **User Story:** As a player, I can watch and participate in AWS-sponsored
    Twitch streams that demonstrate different levels and training.
  - Initial expectation is that a single Community Manager would own this space
    and would expand as need/popularity increases. Would coordinate with Project
    Manager.
- Discord Server
  - **Priority:** Low
  - **Complexity:** Low
  - **User Story:** As a player, I can participate in a moderated community of
    other players to share ideas, learnings, and suggestions.
  - Initial expectation is that a single Community Manager would own this space
    and would expand as need/popularity increases. Would coordinate with Project
    Manager.
- Conference Sessions
  - **Priority:** Medium
  - **Complexity:** Low
  - **User Story:** As a player, I can participate in game sessions during
    conferences such as re:Invent.
  - Initial expectation is that a single Community Manager would own this space
    and would expand as need and popularity increases. Would coordinate with
    Project Manager.
- Public Roadmap
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I am able to view a public-facing roadmap of
    features and bug-fixes, and can contribute to them.
  - Not related to the game or programming, but critical from a socialization
    perspective. This would be hosted on GitHub similar to the AWS
    CloudFormation coverage roadmap.
- Feedback Submission
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can submit feedback in-game, with the option
    to provide a copy of recent logs.
  - This needs to go to a ticketing system of some form (ZenDesk?).

## AWS Mechanics

- Visual Parameters
  - **Priority:** High
  - **Complexity:** Medium
  - **User Story:** As a player, I can configure AWS resources using visual
    parameters instead of text-based input (where possible).
  - Some AWS resource properties can be represented as 3D features that can be
    manipulated by the player (especially helpful in VR where typing is
    cumbersome).
  - Examples:
    - Select from list => Rotating dial
    - On/off (boolean) => Switch or button
  - TBD - How to best represent these controls on the AWS resources themselves.
    - Have them appear above/below the resource as a control panel.
    - Have them appear in the player's hand as a control panel.
- Text Parameters
  - **Priority:** High
  - **Complexity:** Low
  - **User Story:** As a player, I can configure AWS resources usign text input
    wherever visual parameters are not possible/sensible.
  - Inputs such as URLs, JSON/YAML, etc. Would need to be part of the control
    panel for visual parameters.
- Resource Parameters
  - **Priority:** High
  - **Complexity:** Low
  - **User Story:** As a player, I can select from existing AWS resources in my
    account when needed as inputs for other resource configurations.
  - This would need to be represented visually to the player in some fashion.
    The player should have the ability to select resources they have created in
    the game environment but have not yet launched. This will prevent resources
    with unmet dependencies from being launched. TBD - How to highlight or call
    out the resource that is being referenced as a property value.
  - Examples:
    - Select existing IAM policies when creating a role.
    - Select existing subnets when creating an Auto Scaling group.
- Resource Create
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can create a "blank" instance of a resource.
  - This resource requires configuration before it can be launched. Resource
    properties marked as required must be set before the resource can launch.
- Resource Configure
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can configure various properties of a
    resource I created, or one that is already launched.
  - This is done before a launch/update is made, and stored as properties of the
    resource instance.
- Resource Launch
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can launch a configured resource.
  - If AWS integration is enabled, the launch is sent to the configured AWS
    account, otherwise it is simply treated as successful. If the resource
    references other resources that have been created but not launched, the
    option to launch is disabled. If required properties are not set, the option
    to launch is disabled.
- Resource Update
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can update a launched resource.
  - The player would select the launched resource and be able to see editable
    properties. After making edits (same as Resource Configuration), they can
    update the resource. If AWS integration is enabled, the update is sent to
    the configured AWS account, otherwise it is treated as successful If the
    resource references other resources that have been created but not launched,
    the option to update is disabled. If required properties are not set, the
    option to update is disabled.
- Resource Terminate
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can terminate a resource.
  - The player would select the resource and then the option to terminate. If
    the resource is depended on by other resources, the option to terminate is
    disabled. If the resource has been created but not launched, the deletion is
    treated as successful. If AWS integration is enabled, the terminate is sent
    to the configured AWS account.
- Launch Failure Errors
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can see when resources fail to launch.
  - The resource will animate and play a looping sound effect when the player is
    in range.
- Update Failure Errors
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can see when resources fail to update.
  - The resource will animate and play a looping sound effect when the player is
    in range. If the resource is functional after the update fails, the player
    can choose to ""restore"" the resource to it's last good state (i.e. an S3
    bucket policy update can fail, but will still allow the bucket to function
    with its last good configuration).
- Termination Failure Errors
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can see when resources fail to terminate.
  - The resource will animate and play a looping sound effect when the player is
    in range. If the resource is functonal after the termination fails, the
    player can choose to ""restore"" the resource to it's last good state. The
    player can choose to retry termination.

## View Filters

- Operational Excellence
  - **Priority:** High
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to enable a camera filter that will
    show me what resource(s) violate one or more rules of the Operational
    Excellence pillar.
  - When the player defeats the boss for this pillar, this filter is enabled as
    a new ability.
- Security
  - **Priority:** High
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to enable a camera filter that will
    show me what resource(s) violate one or more rules of the Security pillar.
  - When the player defeats the boss for this pillar, this filter is enabled as
    a new ability.
- Reliability
  - **Priority:** High
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to enable a camera filter that will
    show me what resource(s) violate one or more rules of the Reliability
    pillar.
  - When the player defeats the boss for this pillar, this filter is enabled as
    a new ability.
- Performance Efficiency
  - **Priority:** High
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to enable a camera filter that will
    show me what resource(s) violate one or more rules of the Performance
    Efficiency pillar.
  - When the player defeats the boss for this pillar, this filter is enabled as
    a new ability.
- Cost Optimization
  - **Priority:** High
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to enable a camera filter that will
    show me what resource(s) violate one or more rules of the Cost Optimization
    pillar.
  - When the player defeats the boss for this pillar, this filter is enabled as
    a new ability.
- Resource Tagging
  - **Priority:** Low
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to enable a camera filter that will
    show me only resource(s) with a tag that I provide.
  - This should be a starting ability.

## CHLOE Companion

- Launch Animations
  - **Priority:** Medium
  - **Complexity:** High
  - **User Story:** As a player, I am able to watch CHLOE create new AWS
    resources.
  - When a new AWS resource is launched, CHLOE performs a creation animation
    specific to that resource family (storage, serverless, machine learning,
    etc.). Later, we may want to make this more specific to the type of
    resource, not the family."
- Update Animations
  - **Priority:** Medium
  - **Complexity:** High
  - **User Story:** As a player, I am able to watch CHLOE update existing AWS
    resources.
  - When an existing AWS resource is updated, CHLOE performs an update animation
    specific to that resource family (storage, serverless, machine learning,
    etc.). Later, we may want to make this more specific to the type of
    resource, not the family.
- Terminate Animations
  - **Priority:** Medium
  - **Complexity:** High
  - **User Story:** As a player, I am able to watch CHLOE terminate existing AWS
    resources.
  - When an existing AWS resource is terminated, CHLOE performs an update
    animation specific to that resource family (storage, serverless, machine
    learning, etc.). Later, we may want to make this more specific to the type
    of resource, not the family.
- Idle Animations
  - **Priority:** Low
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to watch CHLOE perform idle
    activities.
  - TBD - Some kind of activities. Generally just for entertainment purposes.
- Pet Animation
  - **Priority:** Very High
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to pet CHLOE.
  - In general, the internet does not react well if you can't pet the local
    fauna...
- Subtitles
  - **Priority:** High
  - **Complexity:** Medium
  - **User Story:** As a player, I can read CHLOE's speech as subtitles.
  - The game will not use recorded/generated speech except what is included in
    learning videos.
- Interaction - What is this for?
  - **Priority:** Medium
  - **Complexity:** High
  - **User Story:** As a player, I can interact with CHLOE and ask her what
    specific AWS resources are used for.
  - When doing so, the player is provided with an animated demonstration of
    common use-cases that implement this resource type. High complexity due to
    the animation requirements for these demonstrations.
- Interaction - Where can I learn more?
  - **Priority:** Medium
  - **Complexity:** High
  - **User Story:** As a player, I can interact with CHLOE and ask her where I
    can find more training about a particular resource or resource property.
  - When doing so, the player is provided with various AWS resources
    (documentation, video, training modules from aws.training, etc.) that are
    specific to the resource type or resource property in question. The
    intention is to reduce the amount of "Googling" that builders must do.
  - Example: If the player asks CHLOE about the Canned ACL property of an Amazon
    S3 bucket, she will provide them with various documentation links relevant
    to that specific property.
- Interaction - How do I?
  - **Priority:** Medium
  - **Complexity:** High
  - **User Story:** As a player, I can interact with CHLOE and ask her how to
    build common workloads.
  - The player can choose from a searchable list of available scenarios (i.e.
    "How do I...create a static website with CloudFront integraton?").
  - CHLOE will demonstrate the required architecture and request/response flow.
    No resources are created automatically in the player's linked account(s).
  - After the demonstration completes, the player has the option to modify the
    configuration of each involved resource and launch them. From the game
    engine perspective, the AWS resources are created with some default
    configuration as specified by the workload, but they are not launched yet.
    The player must choose to launch them after viewing the configuration."
- Launch/Update/Termination Failure Notification
  - **Priority:** Low
  - **Complexity:** Medium
  - **User Story:** As a player, I am alerted by CHLOE when resources I created
    fail to launch in my configured AWS account.
  - Notification only happens for resources the player originally created (i.e.
    not for EC2 instances launched automatically by AWS Auto Scaling).
  - This would be implemented as a notification in the HUD. Opening the
    notification would call focus on CHLOE, who would hover around the failed
    resource.
  - Notification can be disabled.

## Metrics and Data Collection

- Data Aggregation Service
  - **Priority:** High
  - **Complexity:** Medium
  - **User Story:**As a product owner, I am able to track metrics and data
    stored in a data aggregation service.
  - We need a data warehouse. Need to see if services like Steam and Epic
    already provide this for developers.
- Customer Events
  - **Priority:** High
  - **Complexity:** Low
  - **User Story:** As a product owner, I am able to track and report on how
    many customer-requested events are scheduled, cancelled, and delivered.
  - Needed to report on the success of the project.
- Internal Events
  - **Priority:** High
  - **Complexity:** Low
  - **User Story:** As a product owner, I am able to track and report on how
    many AWS-managed events are scheduled, cancelled, and delivered.
  - Needed to report on the success of the project.
- Downloads
  - **Priority:** High
  - **Complexity:** Low
  - **User Story:** As a product owner, I am able to track and report on how
    many times the game has been downloaded.
  - Needed to report on the success of the project.
- System Diagnostics
  - **Priority:** High
  - **Complexity:** Low
  - **User Story:** As a product owner, I am able to track and report on the
    system specifications for players installing the game.
  - Aggregated as counts per different hardware/OS component.
- Levels Completed
  - **Priority:** High
  - **Complexity:** Low
  - **User Story:** As a product owner, I am able to track what levels have been
    completed by players.
  - Aggregated count per level, filterable by complete/incomplete.
- Resources Launched
  - **Priority:** High
  - **Complexity:** Medium
  - **User Story:** As a product owner, I am able to track aggregated data on
    the types and quantities of resources launched by players.
  - Aggregated count per service, per resource. Potentially include geo if
    possible.
- Customer Feedback
  - **Priority:** High
  - **Complexity:** Low
  - **User Story:** As a product owner, I am able to track and report on
    customer feedback surveys provided in-game.
  - Aggregated metrics per question. Anonymized answers to text questions.
- Play Time
  - **Priority:** High
  - **Complexity:** Low
  - **User Story:** As a product owner, I am able to track and report on play
    time.
  - Aggregated per level, averages per player.
- Monitoring and SLAs
  - **Priority:** High
  - **Complexity:** Medium
  - **User Story:**
  - TBD - Add info about what is tracked and alarmed on.
- Error Handling
  - **Priority:** High
  - **Complexity:** Medium
  - **User Story:**
  - Add info about what error reporting. Errors should be easy for the game team
    to identify from a screenshot in a foreign language. Should include a
    numeric code or friendly string to identify the source.
  - Also need the ability to send crash diagnostics.

## Nice to Haves

- Main Menu - Language
  - **Priority:** Critical
  - **Complexity:** High
  - **User Story:** As a player, I can select the language of the game in the
    settings menu.
  - This affects localization and generated text, as well as recorded videos
    (i.e. content streamed from YouTube). TBD - Can we generate localized text
    using Amazon Translate.
- Early Level Exit
  - **Priority:** Low
  - **Complexity:** Medium
  - **User Story:** As a player, if I exit a level early my progress is saved so
    that I can restart from the current state.
- CHLOE Customizations
  - **Priority:** Low
  - **Complexity:** High
  - **User Story:** As a player, I am able to unlock and apply customizations to
    CHLOE after completing certain badges and achievements.
  - These can be considered unlockable content that the player can use to
    customize CHLOE.
  - Examples:
    - Color changes
    - Animations
    - Avatar customizations (hats, clothes)
- Shareable Badges
  - **Priority:** Low
  - **Complexity:** High
  - **User Story:** As a player, I can share badges for completion of specific
    learning(s) to social media profiles.
  - This depends heavily on the type of learning we are trying to capture with
    CHLOE. Path-based learning is more suited to having sharable progress such
    as this, i.e. "I can share by DevOps badge after completing the DevOps
    learning path." We could also go the direction of deep-dive badges instead,
    i.e. "I completed AWS CloudFormation deep-dive troubleshooting."
- Single-Use CHLOE Codes
  - **Priority:** Medium
  - **Complexity:** High
  - **User Story:** As a player, I can redeem single-use codes from events and
    livestreams to unlock in-game rewards.
  - These can be considered unlockable content that the player can use to
    customize CHLOE. These should be more exclusive than the ones that can be
    unlocked through normal gameplay.
  - Examples:
    - Alternative CHLOE meshes (different animals).
- Single-Use Avatar Codes
  - **Priority:** Low
  - **Complexity:** Medium
  - **User Story:** As a player, I can redeem single-use codes from events and
    livestreams to unlock avatar customizations.
  - These should be exclusive to such events. TBD - Could they match the swag
    provided at those events?
- MFA Support
  - **Priority:** Low
  - **Complexity:** Low
  - **User Story:** As a player, I am able to link AWS account(s) that require
    multi-factor authentication (MFA).
  - Would require some input field to provide the MFA token any time the
    temporary credentials expire. Would require capturing the error, prompting
    for MFA, and retrying the action.
- Manual Resource Grouping
  - **Priority:** High
  - **Complexity:** High
  - **User Story:** As a player, I can group AWS resources in the environment
    based on my preferences.
  - Groupings can be done to logically organize infrastructure in a way that
    makes sense to the player. This would be stored locally in player
    preferences. We would want to investigate storing this in tags or another
    data source so that multiple players linked to the same AWS account can see
    the same presentation.
- Resource Errors
  - **Priority:** Medium
  - **Complexity:** High
  - **User Story:** As a player, I can see **human-readable details** when a
    resource fails to launch, update, or terminate.
  - Players need to see the API error results when AWS actions fail. The API
    response returned by some services is cryptic at best. We would want to
    implement logic to provide more human-readable output alongside the actual
    response.
- AWS Resource Onboarding
  - **Priority:** Critical
  - **Complexity:** High
  - **User Story:** As a developer, I can use an interface to onboard new
    resources and features into the game.
  - Onboarding a new resource would require:
    - Mesh
    - CRUD APIs
    - Properties
  - Onboarding a new property would require:
    - Property Type
    - Allowed Values (optional)
    - 3D Control Type
- Demo Architecture Onboarding
  - **Priority:** Critical
  - **Complexity:** High
  - **User Story:** As a player, I can access an interface to create new
    architecture demonstrations to be used by CHLOE.
  - To create an architecture demonstration, users need to be able to define the
    architecture, order of resource creation, request flow, CHLOE dialog, and
    more.
- AWS Organizations Support
  - **Priority:** Critical
  - **Complexity:** Medium
  - **User Story:** As a player, I am able to create, read, update, and delete
    (CRUD) AWS Organizations resources.
  - This will likely require a spearate scene/area for management in the game
    world. Will need to be able to manage accounts, OUs, etc., so it would make
    more sense to do that in a scene where the resources within the accounts are
    not visible (like an overworld). One idea is having each member account
    being a portal to a different scene. Not sure how useful that would be
    compared to seeing more of what is going on across accounts.
- Resource Sync - Organizations
  - **Priority:** Critical
  - **Complexity:** Very High
  - **User Story:** As a player, I can configure my game client to automatically
    sync with all accounts in my organization.
  - TBD: Will this require launching resources in the customer account? For AWS
    Organizations accounts, need to determine if this would require resources
    launched in every account, or just the management account. **It is critical
    that this be fast. It is not useful to have to wait 5-10 minutes for this to
    sync.**"
- Multiple AWS Profile Support
  - **Priority:** Medium
  - **Complexity:** High
  - **User Story:** As a player, I can select more than one AWS account to
    simulate at the same time.
  - Different from AWS Organizations support. In this case it's a random
    selection of AWS accounts the player can access.
- AWS CloudFormation Template Generation
  - **Priority:** Low
  - **Complexity:** Medium
  - **User Story:** As a player, I can select specific resources and generate a
    deployable AWS CloudFormation template from them.
  - Uniquely identifying information about those resources would be removed.
    Requires further investigation with customers.
- AWS CloudFormation Template Import
  - **Priority:** Low
  - **Complexity:** Medium
  - **User Story:** As a player, I can import an AWS CloudFormation template to
    visualize in the game.
  - Requires further investigation with customers.
- Framework Resources
  - **Priority:** Low
  - **Complexity:** Low
  - **User Story:** As a player, I can save "framework" resources in a list of
    favorites.
  - A framework resource is a skeleton resource with some default configurations
    that makes it easier to deploy. Requires further investigation with
    customers.
- Multi-Account Organizations Support
  - **Priority:** Critical
  - **Complexity:** Very High
  - **User Story:** As a player, I can navigate through multiple AWS accounts in
    my AWS Organization while in Simulation Mode.
  - TBD - How do we want to present this? In a sense, each AWS account is it's
    own "world", but customers do want multi-account visualization. Think of
    small, medium, large, and very large scales for both account numbers and
    underlying resources.
- Account Activity Replay
  - **Priority:** High
  - **Complexity:** Very High
  - **User Story:** As a player, I can use simulation mode to "replay" the
    history of an AWS account.
  - A replay experience would allow the player to step through the changes that
    took place in an AWS account over time. This is especially useful for
    debugging complex scenarios such as Black Friday outages for an e-commerce
    site. Would require customer enable recording in some form or another
    (CloudTrail potentially?).
- "What If" Analysis
  - **Priority:** High
  - **Complexity:** Very High
  - **User Story:** As a player, I can propose multiple changes to an AWS
    account to view their impacts.
  - Logically similar to an AWS CloudFormation change set, customers want to be
    able to propose changes to infrastructure and see impacts. Requires further
    investigation with customers.
- Environment Map
  - **Priority:** Low
  - **Complexity:** Medium
  - **User Story:** As a player, I can view a map of the environment.
  - The map shows different AWS account(s), region(s), and other container
    resources. The amount of data displayed is dependent on the "size" of the
    environment based on the number of accounts and resources.
- Environment Map - Resource Performance Heatmaps
  - **Priority:** Low
  - **Complexity:** Medium
  - **User Story:** As a player, I can use the world map to see a heatmap of
    performance data.
  - Integration with CloudWatch to heatmap performance, request count, etc?
- Teleport
  - **Priority:** Low
  - **Complexity:** Low
  - **User Story:** As a player, I can teleport to a location of my choosing.
  - From the map screen, the player can select the location they would like to
    transport to.
- Solution Showcase
  - **Priority:** High
  - **Complexity:** High
  - **User Story:** As a player, I can access game worlds that demonstrate
    solutions specific to various functional domains.
  - The player would be able to select from a list of functional domains
    (Serverless, Machine Learning, DevOps, etc.) and load a corresponding game
    world. The game world would contain a number of solutions related to this
    functional domain (i.e. Serverless => Single page static website using
    Amazon S3, Amazon API Gateway, Amazon Cognito, etc.). A primary technical
    hurdle of this will be the regular maintenance of the solutions. As an
    example, the AWS QuickStarts solutions regularly do not work for customers
    after new services and features are released.
- Workshop Creations - Sharing
  - **Priority:** High
  - **Complexity:** High
  - **User Story:** As a player, I can share workloads I created to a social
    platform.
  - Potentially integrate with Steam Workshop or a self-hosted location.
    Security will be a **major** concern here.
- Workshop Creations - Consuming
  - **Priority:** High
  - **Complexity:** High
  - **User Story:** As a player, I can import and launch workloads others
    created and shared on a social platform.
  - Potentially integrate with Steam Workshop or a self-hosted location.
    Security will be a **major** concern here.
- Community Challenges
  - **Priority:** Medium
  - **Complexity:** High
  - **User Story:** As a player, I can participate in one or more community
    challenges.
  - Community challenges involve some activity that is performed by many
    players, such as "remove public access for X number of S3 buckets". Rewards
    for completion of the challenge would be unlocked for the entire community,
    not just the participants. Need to carefully toe the line on this, as the
    challenges **must not** seem like an attempt to get customers to launch more
    resources and increase their bill. They should be focused on optimization,
    cost reduction, etc.
- Real-Life Guides
  - **Priority:** Low
  - **Complexity:** High
  - **User Story:** As an experienced player, I can sign up as a guide to help
    less experienced players in-game.
  - Other than being a guide, players should get some kind of
    recognition/achievement for this (customizations, models, etc.). Should also
    allow "helped" players to submit upvotes or other ranking feedback for
    guides.
- World Events
  - **Priority:** Low
  - **Complexity:** Medium
  - **User Story:** As a player, I will receive notifications for "world events"
    that occur while playing game levels.
  - World events would be randomized, optional, and potentially unrelated to the
    level in question. They would tie to the overall story of assisting the
    company with various IT/AWS tasks, and would serve as "bite-sized learning"
    opportunities. TBD - Need to flesh this out further and do customer
    research. Would player's like this?
- Localization Support
  - **Priority:** Medium
  - **Complexity:** High
  - **User Story:** As a player, I can change the game to a language of my
    preference.
  - If the game gains enough traction we could opt for paying a third party to
    handle localization, or generate it using Amazon Translate.
- Voiced Lines
  - **Priority:** Low
  - **Complexity:** Medium
  - **User Story:** As a player, I can enable audio speech for the CHLOE
    companion.
  - If the game receives enough support, we would want to include either
    recorded or generated audio lines for the CHLOE character. Would need to be
    careful about this though, the services change too much for recording to be
    easy. Automation will likely be best.
- Music - Third Party Support
  - **Priority:** Low
  - **Complexity:** Medium
  - **User Story:** As a player, I can connect to and control my third party
    music applications from within the game.
  - Would it be possible to support players like Spotify, Pandora, iTunes, etc.?
- Multiplayer - Simulation Mode
  - **Priority:** Low
  - **Complexity:** High
  - **User Story:** As a player, I can play with others in Simulation Mode.
- Multiplayer - Simulation Mode - Player Persistence
  - **Priority:** Low
  - **Complexity:** High
  - **User Story:** As a player, I can see other players who are accessing the
    same AWS account(s) as I am.
  - The big question with this is how do we/players determine when to allow
    multiplayer.
    - Do players need to be accessing the exact same list of AWS accounts?
    - Do we restrict this to single AWS accounts at a time?
    - How will players invite one another to sessions?
    - Should players be able to disable multiplayer for themselves or their AWS
      accounts?
    - How do we make sure customers are comfortable with this?"
- Multiplayer - Simulation Mode - Text Chat
  - **Priority:** Low
  - **Complexity:** High
  - **User Story:** As a player, I can use a keyboard to chat with other players
    who are accessing the same AWS account(s) that I am.
  - Customers should be able to log chat transcripts to their accounts.
  - We would need to consider spam, abuse, etc.
- Multiplayer - Simulation Mode - Voice Chat
  - **Priority:** Low
  - **Complexity:** High
  - **User Story:** As a player, I can use a microphone and speakers to talk to
    and listen to other players.
- SNS Hooks
  - **Priority:** Low
  - **Complexity:** Medium
  - **User Story:** As a player, I can use Amazon SNS to send notifications to
    external systems about what is happening inside of Simulation Mode.
  - Need to research with customers. How would they want to use Simulation Mode
    in relation to external systems? Thinking Slack, Discord, etc. for
    notifications, but what else?
- Alternative Control Support
  - See: Able Gamer's Charity. TBD - More specifics around different controller
    support.
- Event Mode
  - **Priority:** Critical
  - **Complexity:** High
  - **User Story:** As a player, I can use Event Mode to connect to
    workshop/hackathon events. AWS has these as Jams and GameDays.
  - TBD - What would this experience look like? In Event Mode:
    - CHLOE is disabled (players can choose to re-enable her).
    - Resource synchronization is enabled.
    - Objective tracking is enabled
- Event Mode - Objective Tracking
  - **Priority:** Critical
  - **Complexity:** High
  - **User Story:** As a player, I am presented with a tracked list of
    objectives while playing in Event Mode.
  - What does this experience look like? Objectives are provided as a
    CloudFormation-like template that describes the needed resources, their
    configuration, objective text, and other metadata. Each objective is
    provided as a list item with the text and needed resource state. Objectives
    can also be evaluated against provided scripts.
- Challenge Levels
  - **Priority:** Medium
  - **Complexity:** High
  - **User Story:** As a player, I can access multiple challenge levels that
    test my skill in particular domains or use cases.
  - Challenge levels are positioned as specific tasks that the player must
    achieve within specific constraints. These are meant as expert-level tests
    of skill and knowledge. Logically similar to "endgame" content in games. Not
    specifically story-related, but very difficult challenges.
  - Example: Create a highly available, asynchronous thumbnail creation stack
    for the lowest possible cost.

## Virtual Reality

- Player - Open/Close Menu
  - **Priority:** Medium
  - **Complexity:** Low
  - **User Story:** As a player, I can hear the sound of opening and closing the
    menus.
  - Opening/closing the menu is done via hand gesture. The sound effect would be
    played when the gesture is recognized (would need to handle edge cases like
    rapidly opening and closing).
- Main Menu - Settings
  - **Priority:** Critical
  - **Complexity:** Medium
  - **User Story:** As a player, I can adjust preferences such as controls,
    graphics quality, sound levels, and more.
  - Not an exhaustive list, but players should be able to change:
    - Controls (VR): Look Sensitivity, Dominant Hand
- VR Controls - Player (Seated)
  - **Priority:** Critical
  - **Complexity:** High
  - **User Story:** As a player, I can control my avatar using a head mounted
    display (HMD) and hand controllers.
  - Actions:
    - Move (point and teleport)
    - Fly
    - Look
    - Interact
    - Menu (anchored to hand)
    - Typing (virtual keyboard)
- VR Controls - Player (Standing)
  - **Priority:** Critical
  - **Complexity:** High
  - **User Story:** As a player, I can control my avatar using a head mounted
    display (HMD) and hand tracking.
  - Actions:
    - Move (point and teleport)
    - Fly
    - Look
    - Interact
    - Menu (anchored to hand)
    - Typing (virtual keyboard)
- VR Controls - Player (Omni-Directional Treadmill)
  - **Priority:** Critical
  - **Complexity:** High
  - **User Story:** As a player, I can use an omni-directional treadmill for
    movement in VR.
  - Actions:
    - Move (walk)
    - Fly
    - Look
    - Interact
    - Menu (anchored to hand)
    - Typing (virtual keyboard)"
- VR Omni-Directional Teadmill (ODT) Support
  - **Priority:** High
  - **Complexity:** High
  - **User Story:** As a player, I can use an omni-directional treadmill to
    navigate within the environment.
  - Investigating various options:
    - ["True" ODTs](https://www.infinadeck.com/)
    - ["Slidemills"](https://www.kat-vr.com/products/kat-walk-c)
    - ["Slidemills" with Anchors](https://www.kat-vr.com/products/kat-walk-premium-vr-treadmill)
    - [Walk-On-Spot System](https://www.kat-vr.com/products/kat-loco-s)
  - Likely would need to live compare for feel, portability, setup/teardown,
    etc.
- VR ODT Arena
  - **Priority:** High
  - **Complexity:** High
  - For big conference events, using a
    [VR Arena](https://www.kat-vr.com/pages/vr_arena).
- Menu - Settings
  - **Priority:** Critical
  - **Complexity:** Medium
  - **User Story:** As a player, I can adjust preferences such as controls,
    graphics quality, sound levels, and more.
  - Not an exhaustive list, but players should be able to change:
    - Controls (VR): Look Sensitivity, Dominant Hand
- AWS Resource Selection
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can open a menu to select the AWS resource I
    want to create.
  - Players can filter by specific AWS services, and can see preview information
    about the service and resource (text, instructional videos, use cases,
    etc.).
  - Implemented in world space.
  - Menu originates from player's non-dominant hand.
  - Preview information originates from CHLOE and moves to stay in player FOV
    until dismissed.
- AWS Resource Configuration
  - **Priority:** Critical
  - **Complexity:** Low
  - **User Story:** As a player, I can open a menu to modify the configuration
    of an AWS resource I am creating.
  - Resource properties are rendered in this menu based on the type (i.e.
    boolean, select from list, editable list, text, etc.).
  - Implemented in world space from the resource in question.

## Rejected

- Leaderboards
  - **User Story:** As a player, I can view a leaderboard to see my local/global
    ranking compared to other players.
  - This exposes potential security concerns. If a player has a low
    Well-Architected ranking and is doxxed by other players, this could expose
    unecessary security risk for the doxxed player/company.
- Root User Login
  - **User Story:** As a player, I can link an AWS account by authenticating as
    the root username and password.
  - Huge security risk. Automatic **NO**.
- Access/Secret Key Login
  - **User Story:** As a player, I can link an AWS account by providing an IAM
    user access key ID and secret access key.
  - Huge security risk. Automatic **NO**.
