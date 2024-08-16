<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Documentation</title>
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.45.0/codemirror.min.css" />
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.45.0/theme/dracula.min.css">
  <link rel="stylesheet" href="style.css">
  <link href="https://fonts.googleapis.com/css?family=Roboto:100,300,400,500,700" rel="stylesheet">
</head>
<body>
    <div class="container-fluid documentation">
      <div class="row">
        <div class="col-md-3 col-xl-2 left-sidebar">
          <div class="logo-wrapper">
              <img src="../template/demo_1/src/assets/images/logo.svg" alt="logo" class="img-fluid">
          </div>
          <h5 class="left-menu-title">Documentation</h5>
          <ul class="left-menu">
              <li><a href="#introduction"> Introduction </a></li>
              <li><a href="#fileStructure"> File Structure </a></li>
          </ul>
          <h6 class="left-menu-title">Installation</h6>
          <ul class="left-menu">
              <li><a href="#setupEnvironment"> Setup Environment </a></li>
              <li><a href="#templateInstallation"> Template Installation </a></li>
          </ul>
          <h6 class="left-menu-title">Deployment</h6>
          <ul class="left-menu">
              <li><a href="#deployment"> Deploy React App </a></li>
          </ul>
          <h6 class="left-menu-title">Basic Structure</h6>
          <ul class="left-menu">
              <li><a href="#appComponent"> App Component </a></li>
              <li><a href="#navbar"> Navbar </a></li>
              <li><a href="#settingsPanel"> Setting panel </a></li>
              <li><a href="#leftSidebar">sidebar </a></li>
              <li><a href="#footer"> Footer </a></li>
          </ul>
          <h6 class="left-menu-title">Other Information</h6>
          <ul class="left-menu">
              <li><a href="#customerSupport"> Customer Support </a></li>
          </ul>
        </div>
        <div class="col-md-9 col-xl-10 main-panel">
          <div class="main-panel-wrapper">
              <h2 class="mt-2 text-center font-weight-light text-muted text-uppercase mb-4">Documentation</h2>
              <div class="card grid-margin">
                <div class="card-body">
                  <h3 id="introduction" class="mb-4">Introduction</h3>
                  <p>Corona React Admin is a responsive React template that is based on the CSS framework Bootstrap 4 and it is built with Sass. Sass compiler makes it easier to code and customize. If you are unfamiliar with Bootstrap or Sass, visit their
                      website and read through the documentation. All of Bootstrap components have been modified to fit the style of Corona React Admin and provide a consistent look throughout the template.</p>
                  <p>Before you start working with the template, we suggest you go through the pages that are bundled with the theme. Most of the template example pages contain quick tips on how to create or use a component which can
                      be really helpful when you need to create something on the fly.</p>
                  </div>
              </div>
              <div class="card grid-margin">
                <div class="card-body">
                  <h3 id="fileStructure" class="mb-4">File Structure</h3>
                  <p>Once you have download the package you will see the following folder structure inside the folder.</p>
                  <textarea rows="4" cols="50" class="code-non-editable">
Corona/
├── React
    ├── template
      ├── modern-vertical
          ├── src/
              ├── app/
              ├── assets/
                  ├── images/
                  ├── styles/
              ├── index.js
          ├── public/
          ├── .gitignore
          ├── CHANGELOG.md
          ├── package.json
          ├── README.md
    ├── CHANGELOG.md
    ├── documentation

                  </textarea>
                </div>
              </div>
              <div class="card grid-margin">
                <div class="card-body">
                  <h3>Installation</h3>
                  <h4 id="setupEnvironment" class="pt-4">Set up the Development Environment</h4>
                  <p>Install <a href="https://nodejs.org/en/" target="_blank">Node.js and npm</a> if they are not already on your machine.</p>
                  <h4 id="templateInstallation" class="pt-4">Template Installation</h4>
                  <p>Go to the project directory and install the React local project dependencies.</p>
                  <p>Run <code>npm install</code>. This command install the dependencies in the local <code>node_modules</code> folder.
                      By default, <code>npm install</code> will install all modules listed as dependencies in <code>package.json</code>.</p>
                  <textarea rows="4" cols="50" class="code-non-editable">npm install</textarea>   
                  <textarea rows="4" cols="50" class="code-non-editable">npm start</textarea>                   
                  <p>The <code>npm start</code> command launches the server, watches your files, and rebuilds the app as you make changes to those files.
                   </p>
                  <p>For more detailed information to install the React application, visit this official React <a href="https://reactjs.org/docs/getting-started.html" target="_blank">documentation website</a>.</p>
                </div>
              </div>
              <div class="card grid-margin">
                <div class="card-body">
                  <h3 id="deployment">Deployment</h3>
                  <h4 class="pt-4">Deploy React app </h4>
                  <p>For the simplest deployment, create a production build and copy the output directory to a web server.</p>
                  <p>1. Start with the production build:</p>
                  <textarea rows="4" cols="50" class="code-non-editable">npm run-script build</textarea>   
                  <p>2. Copy everything within the output folder (build/) to a folder on the server.</p>
                </div>
              </div>
              <div class="card grid-margin">
                <div class="card-body">
                  <h3>Basic Structure</h3>
                  <h4 class="pt-4" id="appComponent">App Component</h4>
                  <textarea rows="4" cols="50" class="code-non-editable">
    
      import React from 'react';
      import ReactDOM from 'react-dom';
      import { BrowserRouter } from 'react-router-dom';
      import App from './app/App';
      import * as serviceWorker from './serviceWorker';
      
      ReactDOM.render(
        <BrowserRouter>
          <App />
        </BrowserRouter>
      , document.getElementById('root'));
      
      serviceWorker.unregister();

                  </textarea>
                  <h4 class="pt-4" id="navbar">Navbar</h4>
                  <textarea rows="4" cols="50" class="code-non-editable">

      import React, { Component } from 'react';
      import { Dropdown } from 'react-bootstrap';
      import { Link } from 'react-router-dom';
      
      class Navbar extends Component {
        toggleOffcanvas() {
          document.querySelector('.sidebar-offcanvas').classList.toggle('active');
        }
        toggleRightSidebar() {
          document.querySelector('.right-sidebar').classList.toggle('open');
        }
        render () {
          return (
            <nav className="navbar p-0 fixed-top d-flex flex-row">
              <div className="navbar-brand-wrapper d-flex d-lg-none align-items-center justify-content-center">
                {/* <Link className="navbar-brand brand-logo" to="/"><img src={require('../../assets/images/logo.svg')} alt="logo" /></Link> */}
                <Link className="navbar-brand brand-logo-mini" to="/"><img src={require('../../assets/images/logo-mini.svg')} alt="logo" /></Link>
              </div>
              <div className="navbar-menu-wrapper flex-grow d-flex align-items-stretch">
                <button className="navbar-toggler align-self-center" type="button" onClick={ () => document.body.classList.toggle('sidebar-icon-only') }>
                  <span className="mdi mdi-menu"></span>
                </button>
                <ul className="navbar-nav w-100">
                  <li className="nav-item w-100">
                    <form className="nav-link mt-2 mt-md-0 d-none d-lg-flex search">
                      <input type="text" className="form-control" placeholder="Search products" />
                    </form>
                  </li>
                </ul>
                <ul className="navbar-nav navbar-nav-right">
                  <Dropdown alignRight as="li" className="nav-item d-none d-lg-block">
                      <Dropdown.Toggle className="nav-link btn btn-success create-new-button no-caret">
                      + Create New Project
                      </Dropdown.Toggle>
      
                      <Dropdown.Menu className="navbar-dropdown preview-list">
                        <h6 className="p-3 mb-0">Projects</h6>
                        <Dropdown.Divider />
                        <Dropdown.Item href="!#" onClick={evt =>evt.preventDefault()} className="preview-item">
                          <div className="preview-thumbnail">
                            <div className="preview-icon bg-dark rounded-circle">
                              <i className="mdi mdi-file-outline text-primary"></i>
                            </div>
                          </div>
                          <div className="preview-item-content">
                            <p className="preview-subject ellipsis mb-1">Software Development</p>
                          </div>
                        </Dropdown.Item>
                        <Dropdown.Divider />
                        <Dropdown.Item href="!#" onClick={evt =>evt.preventDefault()} className="preview-item">
                          <div className="preview-thumbnail">
                            <div className="preview-icon bg-dark rounded-circle">
                              <i className="mdi mdi-web text-info"></i>
                            </div>
                          </div>
                          <div className="preview-item-content">
                            <p className="preview-subject ellipsis mb-1">UI Development</p>
                          </div>
                        </Dropdown.Item>
                        <Dropdown.Divider />
                        <Dropdown.Item href="!#" onClick={evt =>evt.preventDefault()} className="preview-item">
                          <div className="preview-thumbnail">
                            <div className="preview-icon bg-dark rounded-circle">
                              <i className="mdi mdi-layers text-danger"></i>
                            </div>
                          </div>
                          <div className="preview-item-content">
                            <p className="preview-subject ellipsis mb-1">Software Testing</p>
                          </div>
                        </Dropdown.Item>
                        <Dropdown.Divider />
                        <p className="p-3 mb-0 text-center">See all projects</p>
                      </Dropdown.Menu>
                    </Dropdown>
                  <li className="nav-item d-none d-lg-block">
                    <a className="nav-link" href="!#" onClick={event => event.preventDefault()}>
                      <i className="mdi mdi-view-grid"></i>
                    </a>
                  </li>
                  <Dropdown alignRight as="li" className="nav-item border-left" >
                    <Dropdown.Toggle as="a" className="nav-link count-indicator cursor-pointer">
                      <i className="mdi mdi-email"></i>
                      <span className="count bg-success"></span>
                    </Dropdown.Toggle>
                    <Dropdown.Menu className="navbar-dropdown preview-list">
                        <h6 className="p-3 mb-0">Messages</h6>
                        <Dropdown.Divider />
                        <Dropdown.Item href="!#" onClick={evt =>evt.preventDefault()} className="preview-item">
                          <div className="preview-thumbnail">
                            <div className="preview-icon bg-dark rounded-circle">
                              <img src={require('../../assets/images/faces/face4.jpg')} alt="profile" className="rounded-circle profile-pic" />
                            </div>
                          </div>
                          <div className="preview-item-content">
                            <p className="preview-subject ellipsis mb-1">Mark send you a message</p>
                            <p className="text-muted mb-0"> 1 Minutes ago </p>
                          </div>
                        </Dropdown.Item>
                        <Dropdown.Divider />
                        <Dropdown.Item href="!#" onClick={evt =>evt.preventDefault()} className="preview-item">
                          <div className="preview-thumbnail">
                            <div className="preview-icon bg-dark rounded-circle">
                              <img src={require('../../assets/images/faces/face2.jpg')} alt="profile" className="rounded-circle profile-pic" />
                            </div>
                          </div>
                          <div className="preview-item-content">
                            <p className="preview-subject ellipsis mb-1">Cregh send you a message</p>
                            <p className="text-muted mb-0"> 15 Minutes ago </p>
                          </div>
                        </Dropdown.Item>
                        <Dropdown.Divider />
                        <Dropdown.Item href="!#" onClick={evt =>evt.preventDefault()} className="preview-item">
                          <div className="preview-thumbnail">
                            <div className="preview-icon bg-dark rounded-circle">
                              <img src={require('../../assets/images/faces/face3.jpg')} alt="profile" className="rounded-circle profile-pic" />
                            </div>
                          </div>
                          <div className="preview-item-content">
                            <p className="preview-subject ellipsis mb-1">Profile picture updated</p>
                            <p className="text-muted mb-0"> 18 Minutes ago </p>
                          </div>
                        </Dropdown.Item>
                        <Dropdown.Divider />
                        <p className="p-3 mb-0 text-center">4 new messages</p>
                      </Dropdown.Menu>
                  </Dropdown>
                  <Dropdown alignRight as="li" className="nav-item border-left">
                    <Dropdown.Toggle as="a" className="nav-link count-indicator cursor-pointer">
                      <i className="mdi mdi-bell"></i>
                      <span className="count bg-danger"></span>
                    </Dropdown.Toggle>
                    <Dropdown.Menu className="dropdown-menu navbar-dropdown preview-list">
                      <h6 className="p-3 mb-0">Notifications</h6>
                      <Dropdown.Divider />
                      <Dropdown.Item className="dropdown-item preview-item" onClick={evt =>evt.preventDefault()}>
                        <div className="preview-thumbnail">
                          <div className="preview-icon bg-dark rounded-circle">
                            <i className="mdi mdi-calendar text-success"></i>
                          </div>
                        </div>
                        <div className="preview-item-content">
                          <p className="preview-subject mb-1">Event today</p>
                          <p className="text-muted ellipsis mb-0">
                            Just a reminder that you have an event today
                          </p>
                        </div>
                      </Dropdown.Item>
                      <Dropdown.Divider />
                      <Dropdown.Item className="dropdown-item preview-item" onClick={evt =>evt.preventDefault()}>
                        <div className="preview-thumbnail">
                          <div className="preview-icon bg-dark rounded-circle">
                            <i className="mdi mdi-settings text-danger"></i>
                          </div>
                        </div>
                        <div className="preview-item-content">
                          <h6 className="preview-subject mb-1">Settings</h6>
                          <p className="text-muted ellipsis mb-0">
                            Update dashboard
                          </p>
                        </div>
                      </Dropdown.Item>
                      <Dropdown.Divider />
                      <Dropdown.Item className="dropdown-item preview-item" onClick={evt =>evt.preventDefault()}>
                        <div className="preview-thumbnail">
                          <div className="preview-icon bg-dark rounded-circle">
                            <i className="mdi mdi-link-variant text-warning"></i>
                          </div>
                        </div>
                        <div className="preview-item-content">
                          <h6 className="preview-subject mb-1">Launch Admin</h6>
                          <p className="text-muted ellipsis mb-0">
                            New admin wow!
                          </p>
                        </div>
                      </Dropdown.Item>
                      <Dropdown.Divider />
                      <p className="p-3 mb-0 text-center">See all notifications</p>
                    </Dropdown.Menu>
                  </Dropdown>
                  <Dropdown alignRight as="li" className="nav-item">
                    <Dropdown.Toggle as="a" className="nav-link cursor-pointer no-caret">
                      <div className="navbar-profile">
                        <img className="img-xs rounded-circle" src={require('../../assets/images/faces/face15.jpg')} alt="profile" />
                        <p className="mb-0 d-none d-sm-block navbar-profile-name">Henry Klein</p>
                        <i className="mdi mdi-menu-down d-none d-sm-block"></i>
                      </div>
                    </Dropdown.Toggle>
      
                    <Dropdown.Menu className="navbar-dropdown preview-list">
                      <h6 className="p-3 mb-0">Profile</h6>
                      <Dropdown.Divider />
                      <Dropdown.Item href="!#" onClick={evt =>evt.preventDefault()} className="preview-item">
                        <div className="preview-thumbnail">
                          <div className="preview-icon bg-dark rounded-circle">
                            <i className="mdi mdi-settings text-success"></i>
                          </div>
                        </div>
                        <div className="preview-item-content">
                          <p className="preview-subject mb-1">Settings</p>
                        </div>
                      </Dropdown.Item>
                      <Dropdown.Divider />
                      <Dropdown.Item href="!#" onClick={evt =>evt.preventDefault()}  className="preview-item">
                        <div className="preview-thumbnail">
                          <div className="preview-icon bg-dark rounded-circle">
                            <i className="mdi mdi-logout text-danger"></i>
                          </div>
                        </div>
                        <div className="preview-item-content">
                          <p className="preview-subject mb-1">Log out</p>
                        </div>
                      </Dropdown.Item>
                      <Dropdown.Divider />
                      <p className="p-3 mb-0 text-center">Advanced settings</p>
                    </Dropdown.Menu>
                  </Dropdown>
                </ul>
                <button className="navbar-toggler navbar-toggler-right d-lg-none align-self-center" type="button" onClick={this.toggleOffcanvas}>
                  <span className="mdi mdi-format-line-spacing"></span>
                </button>
              </div>
            </nav>
          );
        }
      }
      
      export default Navbar;
                    
                    

                  </textarea>
                  <h4 class="pt-4" id="leftSidebar">Sidebar</h4>
                  <textarea rows="4" cols="50" class="code-non-editable">
      import React, { Component } from 'react';
      import { Link, withRouter } from 'react-router-dom';
      import { Collapse, Dropdown } from 'react-bootstrap';
      import { Trans } from 'react-i18next';
      
      class Sidebar extends Component {
      
        state = {};
      
        toggleMenuState(menuState) {
          if (this.state[menuState]) {
            this.setState({[menuState] : false});
          } else if(Object.keys(this.state).length === 0) {
            this.setState({[menuState] : true});
          } else {
            Object.keys(this.state).forEach(i => {
              this.setState({[i]: false});
            });
            this.setState({[menuState] : true}); 
          }
        }
      
        componentDidUpdate(prevProps) {
          if (this.props.location !== prevProps.location) {
            this.onRouteChanged();
          }
        }
      
        onRouteChanged() {
          document.querySelector('#sidebar').classList.remove('active');
          Object.keys(this.state).forEach(i => {
            this.setState({[i]: false});
          });
      
          const dropdownPaths = [
            {path:'/apps', state: 'appsMenuOpen'},
            {path:'/basic-ui', state: 'basicUiMenuOpen'},
            {path:'/form-elements', state: 'formElementsMenuOpen'},
            {path:'/tables', state: 'tablesMenuOpen'},
            {path:'/icons', state: 'iconsMenuOpen'},
            {path:'/charts', state: 'chartsMenuOpen'},
            {path:'/user-pages', state: 'userPagesMenuOpen'},
            {path:'/error-pages', state: 'errorPagesMenuOpen'},
          ];
      
          dropdownPaths.forEach((obj => {
            if (this.isPathActive(obj.path)) {
              this.setState({[obj.state] : true})
            }
          }));
        
        }
      
        render () {
          return (
            <nav className="sidebar sidebar-offcanvas" id="sidebar">
              <div className="sidebar-brand-wrapper d-none d-lg-flex align-items-center justify-content-center fixed-top">
                <a className="sidebar-brand brand-logo" href="index.html"><img src={require('../../assets/images/logo.svg')} alt="logo" /></a>
                <a className="sidebar-brand brand-logo-mini" href="index.html"><img src={require('../../assets/images/logo-mini.svg')} alt="logo" /></a>
              </div>
              <ul className="nav">
                <li className="nav-item profile">
                  <div className="profile-desc">
                    <div className="profile-pic">
                      <div className="count-indicator">
                        <img className="img-xs rounded-circle " src={require('../../assets/images/faces/face15.jpg')} alt="profile" />
                        <span className="count bg-success"></span>
                      </div>
                      <div className="profile-name">
                        <h5 className="mb-0 font-weight-normal"><Trans>Henry Klein</Trans></h5>
                        <span><Trans>Gold Member</Trans></span>
                      </div>
                    </div>
                    <Dropdown alignRight>
                      <Dropdown.Toggle as="a" className="cursor-pointer no-caret">
                        <i className="mdi mdi-dots-vertical"></i>
                      </Dropdown.Toggle>
                      <Dropdown.Menu className="sidebar-dropdown preview-list">
                        <a href="!#" className="dropdown-item preview-item" onClick={evt =>evt.preventDefault()}>
                          <div className="preview-thumbnail">
                            <div className="preview-icon bg-dark rounded-circle">
                              <i className="mdi mdi-settings text-primary"></i>
                            </div>
                          </div>
                          <div className="preview-item-content">
                            <p className="preview-subject ellipsis mb-1 text-small"><Trans>Account settings</Trans></p>
                          </div>
                        </a>
                        <div className="dropdown-divider"></div>
                        <a href="!#" className="dropdown-item preview-item" onClick={evt =>evt.preventDefault()}>
                          <div className="preview-thumbnail">
                            <div className="preview-icon bg-dark rounded-circle">
                              <i className="mdi mdi-onepassword  text-info"></i>
                            </div>
                          </div>
                          <div className="preview-item-content">
                            <p className="preview-subject ellipsis mb-1 text-small"><Trans>Change Password</Trans></p>
                          </div>
                        </a>
                        <div className="dropdown-divider"></div>
                        <a href="!#" className="dropdown-item preview-item" onClick={evt =>evt.preventDefault()}>
                          <div className="preview-thumbnail">
                            <div className="preview-icon bg-dark rounded-circle">
                              <i className="mdi mdi-calendar-today text-success"></i>
                            </div>
                          </div>
                          <div className="preview-item-content">
                            <p className="preview-subject ellipsis mb-1 text-small"><Trans>To-do list</Trans></p>
                          </div>
                        </a>
                      </Dropdown.Menu>
                    </Dropdown>
                  </div>
                </li>
                <li className="nav-item nav-category">
                  <span className="nav-link"><Trans>Navigation</Trans></span>
                </li>
                <li className={ this.isPathActive('/dashboard') ? 'nav-item menu-items active' : 'nav-item menu-items' }>
                  <Link className="nav-link" to="/dashboard">
                    <span className="menu-icon"><i className="mdi mdi-speedometer"></i></span>
                    <span className="menu-title"><Trans>Dashboard</Trans></span>
                  </Link>
                </li>
                <li className={ this.isPathActive('/basic-ui') ? 'nav-item menu-items active' : 'nav-item menu-items' }>
                  <div className={ this.state.basicUiMenuOpen ? 'nav-link menu-expanded' : 'nav-link' } onClick={ () => this.toggleMenuState('basicUiMenuOpen') } data-toggle="collapse">
                    <span className="menu-icon">
                      <i className="mdi mdi-laptop"></i>
                    </span>
                    <span className="menu-title"><Trans>Basic UI Elements</Trans></span>
                    <i className="menu-arrow"></i>
                  </div>
                  <Collapse in={ this.state.basicUiMenuOpen }>
                    <div>
                      <ul className="nav flex-column sub-menu">
                        <li className="nav-item"> <Link className={ this.isPathActive('/basic-ui/buttons') ? 'nav-link active' : 'nav-link' } to="/basic-ui/buttons"><Trans>Buttons</Trans></Link></li>
                        <li className="nav-item"> <Link className={ this.isPathActive('/basic-ui/dropdowns') ? 'nav-link active' : 'nav-link' } to="/basic-ui/dropdowns"><Trans>Dropdowns</Trans></Link></li>
                        <li className="nav-item"> <Link className={ this.isPathActive('/basic-ui/typography') ? 'nav-link active' : 'nav-link' } to="/basic-ui/typography"><Trans>Typography</Trans></Link></li>
                      </ul>
                    </div>
                  </Collapse>
                </li>
                <li className={ this.isPathActive('/form-elements') ? 'nav-item menu-items active' : 'nav-item menu-items' }>
                  <div className={ this.state.formElementsMenuOpen ? 'nav-link menu-expanded' : 'nav-link' } onClick={ () => this.toggleMenuState('formElementsMenuOpen') } data-toggle="collapse">
                    <span className="menu-icon">
                      <i className="mdi mdi-playlist-play"></i>
                    </span>
                    <span className="menu-title"><Trans>Form Elements</Trans></span>
                    <i className="menu-arrow"></i>
                  </div>
                  <Collapse in={ this.state.formElementsMenuOpen }>
                    <div>
                      <ul className="nav flex-column sub-menu">
                        <li className="nav-item"> <Link className={ this.isPathActive('/form-elements/basic-elements') ? 'nav-link active' : 'nav-link' } to="/form-elements/basic-elements"><Trans>Basic Elements</Trans></Link></li>
                      </ul>
                    </div>
                  </Collapse>
                </li>
                <li className={ this.isPathActive('/tables') ? 'nav-item menu-items active' : 'nav-item menu-items' }>
                  <div className={ this.state.tablesMenuOpen ? 'nav-link menu-expanded' : 'nav-link' } onClick={ () => this.toggleMenuState('tablesMenuOpen') } data-toggle="collapse">
                    <span className="menu-icon">
                      <i className="mdi mdi-table-large"></i>
                    </span>
                    <span className="menu-title"><Trans>Tables</Trans></span>
                    <i className="menu-arrow"></i>
                  </div>
                  <Collapse in={ this.state.tablesMenuOpen }>
                    <div>
                      <ul className="nav flex-column sub-menu">
                        <li className="nav-item"> <Link className={ this.isPathActive('/tables/basic-table') ? 'nav-link active' : 'nav-link' } to="/tables/basic-table"><Trans>Basic Table</Trans></Link></li>
                      </ul>
                    </div>
                  </Collapse>
                </li>
                <li className={ this.isPathActive('/charts') ? 'nav-item menu-items active' : 'nav-item menu-items' }>
                  <div className={ this.state.chartsMenuOpen ? 'nav-link menu-expanded' : 'nav-link' } onClick={ () => this.toggleMenuState('chartsMenuOpen') } data-toggle="collapse">
                    <span className="menu-icon">
                      <i className="mdi mdi-chart-bar"></i>
                    </span>
                    <span className="menu-title"><Trans>Charts</Trans></span>
                    <i className="menu-arrow"></i>
                  </div>
                  <Collapse in={ this.state.chartsMenuOpen }>
                    <div>
                      <ul className="nav flex-column sub-menu">
                        <li className="nav-item"> <Link className={ this.isPathActive('/charts/chart-js') ? 'nav-link active' : 'nav-link' } to="/charts/chart-js"><Trans>Chart Js</Trans></Link></li>
                      </ul>
                    </div>
                  </Collapse>
                </li>
                <li className={ this.isPathActive('/icons') ? 'nav-item menu-items active' : 'nav-item menu-items' }>
                  <div className={ this.state.iconsMenuOpen ? 'nav-link menu-expanded' : 'nav-link' } onClick={ () => this.toggleMenuState('iconsMenuOpen') } data-toggle="collapse">
                    <span className="menu-icon">
                      <i className="mdi mdi-contacts"></i>
                    </span>
                    <span className="menu-title"><Trans>Icons</Trans></span>
                    <i className="menu-arrow"></i>
                  </div>
                  <Collapse in={ this.state.iconsMenuOpen }>
                    <div>
                      <ul className="nav flex-column sub-menu">
                        <li className="nav-item"> <Link className={ this.isPathActive('/icons/mdi') ? 'nav-link active' : 'nav-link' } to="/icons/mdi"><Trans>Material</Trans></Link></li>
                      </ul>
                    </div>
                  </Collapse>
                </li>
                <li className={ this.isPathActive('/user-pages') ? 'nav-item menu-items active' : 'nav-item menu-items' }>
                  <div className={ this.state.userPagesMenuOpen ? 'nav-link menu-expanded' : 'nav-link' } onClick={ () => this.toggleMenuState('userPagesMenuOpen') } data-toggle="collapse">
                    <span className="menu-icon">
                      <i className="mdi mdi-security"></i>
                    </span>
                    <span className="menu-title"><Trans>User Pages</Trans></span>
                    <i className="menu-arrow"></i>
                  </div>
                  <Collapse in={ this.state.userPagesMenuOpen }>
                    <div>
                      <ul className="nav flex-column sub-menu">
                        <li className="nav-item"> <Link className={ this.isPathActive('/user-pages/login-1') ? 'nav-link active' : 'nav-link' } to="/user-pages/login-1"><Trans>Login</Trans></Link></li>
                        <li className="nav-item"> <Link className={ this.isPathActive('/user-pages/register-1') ? 'nav-link active' : 'nav-link' } to="/user-pages/register-1"><Trans>Register</Trans></Link></li>
                      </ul>
                    </div>
                  </Collapse>
                </li>
                <li className="nav-item nav-category">
                  <span className="nav-link"><Trans>More</Trans></span>
                </li>
                <li className={ this.isPathActive('/error-pages') ? 'nav-item menu-items active' : 'nav-item menu-items' }>
                  <div className={ this.state.errorPagesMenuOpen ? 'nav-link menu-expanded' : 'nav-link' } onClick={ () => this.toggleMenuState('errorPagesMenuOpen') } data-toggle="collapse">
                    <span className="menu-icon">
                      <i className="mdi mdi-lock"></i>
                    </span>
                    <span className="menu-title"><Trans>Error Pages</Trans></span>
                    <i className="menu-arrow"></i>
                  </div>
                  <Collapse in={ this.state.errorPagesMenuOpen }>
                    <div>
                      <ul className="nav flex-column sub-menu">
                        <li className="nav-item"> <Link className={ this.isPathActive('/error-pages/error-404') ? 'nav-link active' : 'nav-link' } to="/error-pages/error-404">404</Link></li>
                        <li className="nav-item"> <Link className={ this.isPathActive('/error-pages/error-500') ? 'nav-link active' : 'nav-link' } to="/error-pages/error-500">500</Link></li>
                      </ul>
                    </div>
                  </Collapse>
                </li>
                <li className="nav-item menu-items">
                  <a className="nav-link" href="http://bootstrapdash.com/demo/corona-react-free/documentation/documentation.html" rel="noopener noreferrer" target="_blank">
                    <span className="menu-icon">
                      <i className="mdi mdi-file-document-box"></i>
                    </span>
                    <span className="menu-title"><Trans>Documentation</Trans></span>
                  </a>
                </li>
              </ul>
            </nav>
          );
        }
      
        isPathActive(path) {
          return this.props.location.pathname.startsWith(path);
        }
      
        componentDidMount() {
          this.onRouteChanged();
          // add class 'hover-open' to sidebar navitem while hover in sidebar-icon-only menu
          const body = document.querySelector('body');
          document.querySelectorAll('.sidebar .nav-item').forEach((el) => {
            
            el.addEventListener('mouseover', function() {
              if(body.classList.contains('sidebar-icon-only')) {
                el.classList.add('hover-open');
              }
            });
            el.addEventListener('mouseout', function() {
              if(body.classList.contains('sidebar-icon-only')) {
                el.classList.remove('hover-open');
              }
            });
          });
        }
      
      }
      
      export default withRouter(Sidebar);
                  </textarea>
                  <h4 class="pt-4" id="footer">Footer</h4>
                  <textarea rows="4" cols="50" class="code-non-editable">
      import React, { Component } from 'react';
      import { Trans } from 'react-i18next';
      
      class Footer extends Component {
        render () {
          return (
            <footer className="footer">
              <div className="container-fluid">
                <div className="d-sm-flex justify-content-center justify-content-sm-between py-2 w-100">
                  <span className="text-muted text-center text-sm-left d-block d-sm-inline-block">Copyright © <a href="https://www.bootstrapdash.com/" target="_blank" rel="noopener noreferrer">bootstrapdash.com </a>2020</span>
                  <span className="float-none float-sm-right d-block mt-1 mt-sm-0 text-center">Free <a href="https://www.bootstrapdash.com/react-admin-templates/" target="_blank" rel="noopener noreferrer"> react admin </a> templates from BootstrapDash.com.  </span>
                </div>
              </div>
            </footer>
          );
        }
      }
      
      export default Footer;
                  </textarea>
                </div>
              </div>
              <div class="card">
                <div class="card-body">
                  <h3 id="customerSupport" class="mb-4">Customer Support</h3>
                  <p>If you face any issue while building your dashboard with Corona React Admin, please contact us via <a href="https://bootstrapdash.freshdesk.com/support/tickets/new" target="_blank">Bootstrapdash support form</a> .</p>
                  <p>We will respond to you as quickly as we can. Thank you.</p>
                </div>
              </div>
          </div>
        </div>
      </div>
    </div>
    <script src="https://code.jquery.com/jquery-3.3.1.min.js" integrity="sha256-FgpCb/KJQlLNfOu91ta32o/NMZxltwRo8QtmkMRdAu8=" crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.45.0/codemirror.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.45.0/mode/python/python.min.js"></script>
    <script src="script.js"></script>
</body>
</html># first-project
