# Rails Testing Cheatsheet

> 🚌 A community-driven cheatsheet for testing Rails apps. Its all on one page to make it easier to find what you're looking for.

## Capybara

```ruby
visit "/login"

click_link "Home"
click_button "Submit"
click_on "Locator for a button or a link"

fill_in "Username", with: "jane@example.org"

within_element "nav" do
  ...
end

save_and_open_page

expect(page).to have_text "some text"
expect(page).to have_content "some more text"
expect(page).to have_current_path "/login"
expect(page).to have_css "h1", text: "The Headline"
expect(page).to have_link "Register"
```
