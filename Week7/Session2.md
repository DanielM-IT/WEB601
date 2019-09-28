# Week 7 Session 2

Today the focus is on component lifcycles. Like anything else that has a lifecycle, react.js component lifecycles have a beginning and an end. They are first created (mounted on the DOM) grow by being updated and then are unmounted which is their end.
Over the lifecycle of a component different methods can be used at the various stages of the lifecycle. Part of todays session was us having a research into these and creating a repository that contains the different methods usable in a component lifecycle.

Below is an image from 'https://medium.com/@baphemot/understanding-react-react-16-3-component-life-cycle-23129bc7a705' which shows the diferent methods and which phases of the component lifecycle they are used in:
https://drive.google.com/file/d/1fJwabimnl3AuG6daRn-pbymab_190VdR/view

The first section is mounting of the component. This usually starts out by being initialized by the 'constructor()' method.
Next up is the 'render()' method. This is the most used lifecycle method and this is because it must be used in all React classes.It renders the component to the UI and happens during the mounting and updating phases of a components lifecycle.
Other methods which can be implemented during the mounting phase are 'getDerivedStateFromProps()', 'componentDidMount()' and 'comonentWillMount()'.

The methods that can be implemented during the update period are 'getSnapshotBeforeUpdate()', 'shouldComponentUpdate()', 'componentDidUpdate()', and 'componentWillUpdate()'.

For unmounting 'componentWillUnmount()' is used. This unmounts and destroys the component. It is considered a good place to clean up data as a result.


For the end of this session we have been asked to group ourselves into groups of three and prepare to give a thunder talk a week from today. The topic will 
be our choice of any full stack web development. Milton and I have chosen to stick together for this and due to not being able to find a third person for 
our team we will two man the thunder talk. We have chosen to do 'MEAN' as our full stack of choice.
