# Hackathon Page

### [Live Version](https://62c46c073c107938600a202f--playful-jalebi-b268f9.netlify.app/)

A Web App For Hackathon Admin Pannel to demonstrate where your admins can modify challenges easily

## Requirements

- yarn

## Libraries Used

- [React](https://reactjs.org/)
- [React-Ace](https://github.com/securingsincity/react-ace)

## How to run:

1. [Download](https://github.com/blueuwu/RandomRepo/archive/refs/heads/main.zip) or [Clone](https://github.com/blueuwu/RandomRepo.git) the Repository.
2. Run `yarn install` to install the project dependencies.

3. Run `yarn start` to run the app in development mode.

4. App can be seen at: `http://localhost:3000/`

## Page Load Time

Page Load TIme has been calculated by using the [Lighthouse Tool]().

![img](https://user-images.githubusercontent.com/80516804/177378501-702e179c-a6a8-4d80-9774-37feba09a9ba.PNG)
![img](https://user-images.githubusercontent.com/80516804/177378647-5bfbee52-14c1-4979-9d08-669809c46317.PNG)


### Steps taken to Optimize

1. There was render blocking javascript for google font causing delay, used method mentioned [here](https://pagespeedchecklist.com/asynchronous-google-fonts) to overcome the problem.

2. Import for `react-ace` editor was long tasks running during page load, Converted it to Lasy loaded component using `React.lazy()` for code-splitting and delaying it's loading.

3. Only importing used Module in a component from library rather than importing whole library.

## create-react-app

This project was bootstrapped with [Create React App](https://github.com/facebookincubator/create-react-app). You can find more information on how to perform common tasks [here](https://github.com/facebook/create-react-app/blob/master/packages/cra-template/template/README.md).
