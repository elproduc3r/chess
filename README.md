# React Chess

## Unit and Browser testing 
### Unit Testing
Testing is critical for any code that is to be maintained and further developed. My plan for this app would be to setup Code Coverage with jest and set a threshold starting at 95% and adjust if necessary. Then I would create unit tests with React Testing Library (RTL) for each component and sub component (i.e. `src/components/Board/Board.tsx` as well as `src/components/Board/Cell.tsx`).

In addition to the unit testing I would also add `axe` tests for accessibility as well as snapshot tests.

### Browser testing
Since this is a highly interactive application I would also implement Playwright testing to perform more interactive testing in various browsers and test events like clicking and dragging.

Beyond Playwright testing, I think it would be good to setup Storybook with a story for each component. Then with Applitools you can perform Visual Regression testing through Storybook in the pipeline and catch visual changes as well as compare rendering at different device sizes (breakpoints).

![screenshot](https://i.ibb.co/Xt4XTjq/screen.png) 
