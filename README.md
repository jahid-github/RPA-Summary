# RPA-Summary
## Importing Required Modules
from robocorp.tasks import task # Imports Robocorp's task decorator (@task), which marks a function as an automation task.
from robocorp import browser # Imports browser automation features (built on Playwright) for opening, interacting with, and closing web pages.
## Defining an Automation Task
@task
def open_page():
## Navigating to the Website
browser.goto(url)
## Filling the Search Box
page.locator("#search").fill("Mark Pilgrim : Dive into Python")
## Submitting the Search Form
page.evaluate("document.querySelector('#search').form.submit()")
## Taking a Screenshot
browser.screenshot()
