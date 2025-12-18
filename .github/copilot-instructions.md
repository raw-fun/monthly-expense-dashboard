# Copilot Instructions for Monthly Expense Dashboard

## Project Overview
This is a single-page HTML dashboard for tracking monthly expenses for a residential building or community. The dashboard displays service charge collections from members and various expense categories, all in Bengali (Bangla) language.

## Technology Stack
- Pure HTML5 with embedded CSS
- Bengali (Bangla) language for all text content
- Font Awesome icons
- Google Fonts (Hind Siliguri for Bengali text, Inter for numbers)
- No JavaScript framework or build tools required

## Code Style Guidelines

### HTML Structure
- Maintain semantic HTML5 structure
- Use appropriate ARIA labels for accessibility where needed
- Keep all styles in the `<style>` tag within the `<head>` section
- Preserve the existing class naming conventions

### CSS Guidelines
- Use CSS custom properties (CSS variables) defined in `:root` for colors and theme values
- Follow the existing color scheme:
  - Primary: `var(--primary)` (#2563eb - Royal Blue)
  - Success: `var(--success)` (#10b981 - for income/collections)
  - Danger: `var(--danger)` (#ef4444 - for expenses)
  - Maintain existing spacing and sizing conventions
- Ensure print styles remain functional for generating reports

### Language and Content
- **All user-facing text MUST be in Bengali (Bangla) language**
- Use Bengali numerals where appropriate (০১২৩৪৫৬৭৮৯)
- Maintain the formal/respectful tone used in member names (মোঃ, মোছাঃ prefixes)
- When adding new members or expenses, follow the existing naming conventions

### Responsive Design
- Ensure the dashboard works well on desktop, tablet, and mobile devices
- The existing breakpoint at 1024px should be maintained
- Test print functionality when making layout changes

### Data Structure
- Member collection table includes: Name, Flat number, Status, Amount
- Expense items include: Category name, Visual bar indicator, Amount
- All monetary values should be formatted consistently (e.g., ১,০০০/-)

## Common Tasks

### Adding New Members
1. Add a new `<tr>` row in the collection table
2. Include member name, flat number badge, status badge, and amount
3. Update the total collection row at the bottom
4. Update the "X জন সদস্য" count in the card header
5. Update the stats cards at the top to reflect new totals

### Adding New Expense Categories
1. Add a new expense item div with class `expense-item`
2. Include expense name and amount
3. Add a visual bar indicator with appropriate width percentage
4. Update the total expense row at the bottom
5. Update the "Xটি খাত" count in the card header
6. Update the stats cards to reflect new totals

### Updating Colors or Theme
1. Modify CSS custom properties in the `:root` selector
2. Test both light theme and print styles
3. Ensure sufficient contrast for accessibility

## Testing
- Open `index.html` in a web browser to preview changes
- Test the print functionality (Ctrl+P or Cmd+P)
- Verify responsive behavior by resizing the browser window
- Check that all Bengali text displays correctly with proper fonts

## Important Notes
- This is a static dashboard - no backend or database
- Data is hardcoded in the HTML file
- The dashboard is designed for a specific building/community (November 2025 data)
- Maintain the existing visual design and layout structure
- Preserve print functionality as users rely on it for generating reports
