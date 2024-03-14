Sofia Valiante 40191897

## Basic Calculator

## Android App
Method:
protected void applyCustomTheme() {
        binding.commentCoordinatorLayout.setBackgroundColor(mCustomThemeWrapper.getBackgroundColor());
        applyAppBarLayoutAndCollapsingToolbarLayoutAndToolbarTheme(binding.commentAppbarLayout, null, binding.commentToolbar);
        binding.commentParentTitleTextView.setTextColor(customThemeWrapper.getPostTitleColor());
        binding.commentDivider.setBackgroundColor(mCustomThemeWrapper.getDividerColor());
        binding.commentCommentEditText.setTextColor(mCustomThemeWrapper.getCommentColor());
        int secondaryTextColor = mCustomThemeWrapper.getSecondaryTextColor();
        binding.commentCommentEditText.setHintTextColor(secondaryTextColor);
        if (isReplying) {
            parentTextColor = mCustomThemeWrapper.getCommentColor();
        } else {
            parentTextColor = mCustomThemeWrapper.getPostContentColor();
        }
        parentSpoilerBackgroundColor = parentTextColor | 0xFF000000;
        binding.commentAccountNameTextView.setTextColor(mCustomThemeWrapper.getPrimaryTextColor());

        if (typeface != null) {
            binding.commentCommentEditText.setTypeface(typeface);
        }
        if (titleTypeface != null) {
            binding.commentParentTitleTextView.setTypeface(titleTypeface);
        }
    }
}

1) CFG

![code2flow_aotaKM](https://github.com/SOEN345-WINTER2024/cfg-graph-lab-s-vali/assets/91510546/9701a6eb-4d00-46ef-b1f3-dcd5dcdfe3b9)

2) Node coverage
<br> TR = { 1, 2, 3, 4, 5, 6, 7, 8, 9 }
<br> TP = { (1,2,4,5,7,8,9), (1,2,3,5,7,9), (1,2,4,5,6,7,9) }

3) Edge coverage
<br> TR = { (1,2), (2,3), (2,4), (3,5), (4,5), (5,6), (5,7), (6,7), (7,8), (8,9), (7,9) }
<br> TP = { (1,2,4,5,7,9), (1,2,4,5,7,8,9), (1,2,3,5,7,9), (1,2,4,5,6,7,9) }

4) Edge-pair coverage
<br> TR = { [1,2,3], [1,2,4], [2,3,5], [2,4,5], [3,5,6], [3,5,7], [4,5,6], [4,5,7], [5,6,7], [5,7,8], [5,7,9], [6,7,8],  [6,7,9], [7,8,9] }
<br> TP = { [1,2,3], [2,3,5], [3,5,7], [5,7,9], [1,2,4], [2,4,5], [4,5,7], [5,7,9], [1,2,3], [2,3,5], [3,5,6], [5,6,7], [6,7,9], [1,2,4], [2,4,5], [4,5,6], [5,6,7], [6,7,9], [1,2,4], [2,4,5], [4,5,7], [5,7,8], [7,8,9], [1,2,4], [2,4,5], [4,5,6], [5,6,7], [6,7,8], [7,8,9] }

5) 
